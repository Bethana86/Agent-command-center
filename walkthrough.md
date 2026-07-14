# Walkthrough - TCS Agent Command Center

We have built a premium, interactive web application showcasing **"The AI Control Plane as the Anchor for Enterprise AI Governance"** styled as the **TCS Agent Command Center** (aligned with Google's Gemini Enterprise Agent Platform taxonomy).

---

## 📂 Deliverables Created

All code files are located in the subdirectory [ai-control-plane-governance](file:///C:/Users/ASUA/.gemini/antigravity/scratch/ai-control-plane-governance/):

1. **[index.html](file:///C:/Users/ASUA/.gemini/antigravity/scratch/ai-control-plane-governance/index.html)**: High-fidelity layout containing the Control Lanes visualization, the Persona Panel switcher, and the SecOps log.
2. **[style.css](file:///C:/Users/ASUA/.gemini/antigravity/scratch/ai-control-plane-governance/style.css)**: Glassmorphic dark theme (indigo, violet, cyan) with custom animations for packets traversing the six governance lanes.
3. **[app.js](file:///C:/Users/ASUA/.gemini/antigravity/scratch/ai-control-plane-governance/app.js)**: Control logic, background simulator, policy validation rules (PII masking, jailbreak filters, rogue endpoints), budget limits, and a tamper-evident cryptographic SHA-256 ledger.
4. **[README.md](file:///C:/Users/ASUA/.gemini/antigravity/scratch/ai-control-plane-governance/README.md)**: Project description and setup instructions.

---

## ⚡ Features Implemented & Verified

### 1. Separation of Concerns Visualizer
- Color-coded paths matching the 6 governance pillars (Identity & Access, Policy Enforcement, Registration, Observability, Cost Controls, Runtime Intervention).
- Interactive packets (with success `✓` or fail `✗` markers) flow across paths dynamically as tasks are simulated.

### 2. Multi-Persona Perspectives ("One Truth, Multiple Views")
- **Agent Lifecycle Trace View**: Interactive step-by-step lifecycle execution flow of registered agents. Features an **Enterprise Observability Hub** showing real-time metrics for Agent Task Success Rate, average planning latency, Knowledge Hub (RAG) hit rate, active tool uptime (42 MCP endpoints), model distribution, and gateway integration contexts.
- **Risk & Compliance View**: Admin switches to toggle Model Armor shields. Includes a **Risk Gap Map** highlighting regulatory vulnerabilities (GDPR, EU AI Act) when protections are disabled.
- **Cost Tracing & Monitoring View**: Granular cost tracking across categories (total spend today, cached token savings via Gemini caching, tool execution fees, and base API costs) with a **Runaway Agent Loop Simulator** demonstrating automated gateway throttling intervention.
- **Platform Administrator View**: Systems diagnostic metrics, latency chart, and active gateway sessions with pause, throttle, and termination buttons.

### 3. Cryptographic Tamper-Evident Ledger
- Integrates the native browser Web Crypto API.
- Hashes log block metadata recursively (SHA-256 hashing including the previous block hash).
- Includes a "Verify Ledger" integrity check which recalculates the hashes to ensure audit logs have not been retroactively altered.

---

## 🚀 Local Host Verification

We launched a local development server using the Windows Python launcher:
```powershell
py -m http.server 8080
```
The server is currently running in the background.

> [!TIP]
> Access the portal by navigating to **[http://localhost:8080](http://localhost:8080)** in your browser. 
> To test runtime intervention, switch to the **Platform Ops** tab and click **Pause** or **Terminate** on any running session to watch the audit logs intercept the execution in real-time.
