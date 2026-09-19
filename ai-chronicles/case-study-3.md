### 🔹 Case Study 3: AI-Driven Supply Chain Audit — Engineering a Custom Local LLM Vulnerability Scanner for Third-Party Assets

- **Context & Threat Modeling**:
  When required to integrate an unverified, vendor-provided Docker configuration template into my production GitHub ecosystem, my defensive assessment flagged immediate **supply chain risks**. To prevent configuration drift, dependency contamination, and potential credential leaks, I executed an immediate **Infrastructure Isolation Workflow**:
  1. Staged the third-party infrastructure within an air-gapped, isolated repository environment.
  2. Segregated the source code entirely from my primary development identity.
  3. Initiated a automated static application security testing (SAST) pipeline on the vendor asset.

- **Technical Approach: Engineering an AI-Driven SAST Utility**:
  Rather than relying on passive skepticism, I chose to algorithmically quantify the architectural risks. I engineered a custom automated static analysis utility powered by a local Large Language Model via the **Ollama API (Llama 3.2)**, ensuring full data sovereignty and zero data leakage to external clouds.

```text
[Vendor Dockerfile] ──> [Custom Python Parsing Script] ──> [Local Ollama / Llama 3.2 Engine] ──> [Structured JSON Vulnerability Report]
```

By piping the raw configuration parameters and base layer hashes into the local inference engine, I audited the container's supply chain risks. The custom analyzer programmatically flagged high-severity indicators within seconds:

- **Supply Chain Vector Detection**: Identified base image structures matching parameters reminiscent of historical `PHP 8.1.0-dev` backdoor entry points.
- **Unpatched OS Layers (Privilege Escalation Risk)**: Flagged systemic, out-of-date package management definitions (`apt` layers missing mandatory patch upgrades), presenting an unmitigated attack surface for local privilege escalation.

The automated pipeline generated a definitive security alert: _"Review Dockerfile layers immediately; structural dependencies exhibit outdated package patch anomalies and unvalidated base configurations."_

- **Strategic Pivot & Zero-Trust Validation**:
  When internal organizational constraints prevented a comprehensive remediation or advisory patching of these assets, I executed a strategic pivot guided by **Zero-Trust Principles**. Operating under the framework that _no third-party dependency is secure until programmatically verified_, I autonomously expanded my engineering roadmap. I dedicated my computing infrastructure to building a robust, financial-grade authentication engine and actively hunting bugs on the **HackerOne VDP** platform, securing a valid triage within 30 days.

> _"True security sovereignty means writing the tools to verify what the world expects you to trust blindly."_

🔒 Compliance & Asset Protection Notice:To respect the Intellectual Property (IP) and non-disclosure constraints of the educational provider, the original vendor Dockerfile, the specific implementation source code of the custom scanner, and the raw vulnerability logs are omitted from this public repository. This case study serves purely as an architectural methodology blueprint.
