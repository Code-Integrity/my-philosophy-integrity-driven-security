# Case Study 3: AI-Driven Supply Chain Audit — Engineering a Custom Container Vulnerability Scanner 🤖

> _"Don't just be a consumer; be the sovereign of your information."_

---

## 観測と脅威モデル (The Observation & Threat Modeling)

When instructed by the bootcamp coordinator to directly force-push a vendor-provided Docker configuration template into my production GitHub repository, my defensive instincts flagged an immediate risk.

To prevent configuration drift and repository contamination, I instantly executed an **Incident Isolation Protocol**:

1. Provisioned a temporary, isolated burner GitHub account.
2. Isolated the vendor infrastructure completely from my primary development identity.
3. Began an automated audit of the vendor-supplied infrastructure.

---

## 技術的アプローチ: AI駆動型チェッカーの開発 (Technical Approach: AI-Driven Security Auditing)

Instead of relying on passive skepticism, I chose to algorithmically prove the risk. I engineered a custom automated static analysis utility powered by a local Large Language Model via the **Ollama API** (`Llama 3.2`).

```text
[Vendor Dockerfile] ──> [Custom Scanning Script] ──> [Local Ollama / Llama 3.2] ──> [Structured Vulnerability Report]
```

By piping the raw configuration parameters into the local LLM engine, I audited the container's supply chain layers. The automated analyzer flagged high-severity systemic indicators within seconds:

- **Known Supply Chain exploits**: Identified base image components matching critical parameters (reminiscent of historical `PHP 8.1.0-dev` backdoor vectors).
- **Unpatched OS Layers**: Flagged systemic out-of-date package management instructions (`apt` components missing mandatory upgrade and patching logic), presenting an unmitigated attack surface for local privilege escalation.

The engine delivered a definitive alert: _"Review Dockerfile immediately; the infrastructure architecture presents critical outdated package patch anomalies."_

---

## 戦略的決断とゼロトラストの証明 (The Strategic Pivot & Zero-Trust Validation)

Despite presenting these empirical threat logs, the organization continued mass-distribution of the compromised templates without advisory alerts or security configurations.

Recognizing a total collapse of security culture and internal compliance, I executed a hard strategic pivot. I implemented **Zero-Trust Principles**—refusing to assume any tool is safe simply because it originates from an authoritative vendor. I distanced myself from the environment to focus 100% of my compute power on autonomous personal projects, including a financial-grade authentication engine.

---

### 🇯🇵 日本語解説（内容確認用）

スクールが配布したDockerテンプレートファイルを検証なしにメインリポジトリへ流し込む指示を受けた際、私は即座に脅威を感知し、メイン環境の汚染を防ぐために「捨てアカ」への隔離を実行しました。

その上で、不信感を技術的に検証するため、ローカルLLM（Ollama + Llama 3.2）と連携した**「カスタム・コンテナ脆弱性チェッカー」**を独自にスクリプトで開発。配布されたDockerfileの静的解析を行いました。

結果、ローカルAIは「PHP 8.1の潜在的バックドアリスク」や「OSパッケージ（apt）の未パッチによる脆弱性」を即座に検出。感情的な反発ではなく、**「自作ツールとAIによる客観的なログ」**によって環境のリスクを定量化しました。

この深刻なリスクに対して警鐘を鳴らさない組織の姿勢を見切り、私は「配布物だから安全」という前提を疑う**ゼロトラスト（Zero-Trust）**を実践。スクール環境から距離を置き、100%自走して欧州銀行レベルの認証アプリ開発や、HackerOneでの実戦（トリアージ獲得）へと舵を切りました。
