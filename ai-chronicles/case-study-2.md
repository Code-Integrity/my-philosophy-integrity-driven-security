# Case Study 2: Defensive Git Workflows — Rejecting Raw Pushes to the Production Branch 🌿

> _"Never lean on someone else's rail; build your own flight path."_

---

## 観測と違和感 (The Observation & Friction)

While reviewing the bootcamp's GitHub training section, I discovered that the curriculum instructed students to perform direct modifications and raw `git push` operations directly into the `main` branch.

Knowing that the `main` branch represents the canonical, production-ready state of any software architecture, I immediately questioned this practice. Why would an educational institution enforce an anti-pattern that is explicitly forbidden in professional software environments?

---

## AIとの対話とインサイト (The AI Dialogue & Structural Insight)

I utilized AI to dissect the business logic behind this educational shortcut. The dialogue exposed a compromise in the vendor's quality assurance:

- **The Vendor's Shortcut**: Enforcing proper branching strategies, feature branches, code reviews, and Pull Requests (PRs) requires significant educational overhead and mentor time. To artificially accelerate the completion rate and minimize operational costs, the provider chose to prioritize "immediate visual success" over critical standard operating procedures.
- **The Structural Risk**: Direct pushing to `main` completely destabilizes code integrity. A single unvalidated bug or security injection immediately corrupts the production state. It bypasses peer review, creates unresolvable merge conflicts in collaborative environments, and completely violates the foundational concepts of continuous integration and DevSecOps.

---

## 私の立場と誠実さの基準 (My Stance & The Standards of Integrity)

While I complied with the basic task requirements to progress through the curriculum, I refused to adopt this hazardous habit. I established a personal mandate to execute a proper **Defensive Workflow**:

1. **Branch Isolation**: Created dedicated feature branches (`feature/xxx`) for all functional implementations, leaving `main` strictly as the stable production state.
2. **Simulated Pull Requests**: Replicated the professional review process by manually staging, auditing, and executing controlled merges via Pull Requests, documenting code changes transparently.
3. **Sovereign Execution**: True integrity means choosing the correct, standard methodology regardless of the environment's lower expectations. I prioritized mastering long-term industry-standard branch management over short-term curriculum shortcuts.

---

### 🇯🇵 日本語解説（内容確認用）

スクールのカリキュラムにおいて、`main`ブランチへの直接プッシュという危険なアンチパターンが指導されていることに気づきました。プロの現場において`main`は常に本番環境の神聖な成果物を置く場所であり、ガードされるべきです。

AIとの対話を通じて、この指導法の裏にある「教育コスト削減」「形だけの早期卒業」というプロバイダー側の合理性を突き止めました。この方法をそのまま受け入れることは、コードの整合性を崩壊させ、レビュープロセス（コード監査）を形骸化させる野蛮な手法です。

私はこの手抜きに染まることを拒否しました。すべての課題において自主的にフューチャーブランチ（`feature/`）を切り、モックレビュー（模擬プルリクエスト）を行うことで、実務で不可欠な**「防衛的ギットワークフロー（Defensive Git Workflow）」**を体に叩き込みました。
