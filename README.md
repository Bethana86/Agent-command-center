# The AI Control Plane as the Anchor for Enterprise AI Governance

A premium, interactive web application built to demonstrate the **TCS Agent Command Center** as the Anchor for Enterprise AI Governance (aligned with Google's Gemini Enterprise Agent Platform). 

---

## 🌟 Key Pillars of AI Governance Visualized

This application illustrates how security, cost, compliance, and lifecycle audits can be decoupled from the runtime execution of models using GEAP’s architecture:

1. **Identity & Access** (GEAP Tenant Gateway Auth): Asserts least-privilege token credentials before models execute, isolating workloads by tenant, project, and environment.
2. **Policy Enforcement** (GEAP Model Armor): Blocks prompt injection vectors, jailbreak commands, and masks PII (Social Security Numbers, API Keys) on inputs and outputs.
3. **Registration** (GEAP Agent Registry): Maintains the inventory of active models (Gemini 1.5 Pro, Flash, Gemma), agents, and tool permissions.
4. **Observability** (GEAP Compliance Policy Auditor): Audits payloads into a cryptographic, tamper-evident ledger (signed using SHA-256 hashes).
5. **Cost Controls** (GEAP Gateway Billing & Rate Limiter): Enforces limits and budget guardrails per tenant.
6. **Runtime Intervention** (GEAP Runtime Interceptor): Empowers operators to Pause, Throttle, or Terminate workloads dynamically at the Gateway level.

---

## 📂 Project Directory Structure

```
ai-control-plane-governance/
├── index.html     # Skeleton structure, Control Lane visualizer, and Persona Panels
├── style.css      # Custom dark-mode glassmorphic theme (indigo, violet, cyan highlights)
├── app.js         # Core workload simulation engine, cryptographic ledger, and Chart.js mapping
└── README.md      # Setup guide and features overview (this file)
```

---

## 🚀 How to Run the Application Locally

The application is built using standard web standards (HTML5/CSS3/ES6 JS) and has **zero external installations or compilation steps**. It runs in any modern browser.

### Step 1: Open the directory in your shell
```powershell
cd C:\Users\ASUA\.gemini\antigravity\scratch\ai-control-plane-governance
```

### Step 2: Start a lightweight local server
Run any of the following commands depending on what runtime you have installed:

* **Using Python:**
  ```bash
  python -m http.server 8080
  ```
* **Using Node.js (npx):**
  ```bash
  npx http-server -p 8080
  ```

### Step 3: Open in Browser
Navigate to [http://localhost:8080](http://localhost:8080) to access the interactive Governance Control Center.
