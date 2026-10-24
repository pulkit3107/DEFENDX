# DEFENDX // CY-02 — AI Security Reviewer

> **Hackathon Track: CY-02 AI Security Reviewer**  
> **Brand & Experience: DEFENDX — Warm & Soothing Luxury Dark Cybersecurity Platform**

---

## 🛡️ About DEFENDX
*Every software codebase is an interconnected network. A single weak point can compromise the entire structure. DEFENDX reveals what is hidden, traces the risk, and helps developers strengthen every connection before code reaches production.*

### 🎨 Visual Identity & Soothing Warm Dark Palette
- **Palette**: Deep Espresso/Charcoal (`#0E0C13`), Soft Warm Slate (`#16131D`), Warm Amber (`#F59E0B`), Golden Sunset (`#FBBF24`), Terracotta Coral (`#EB5E55`), Soothing Warm Cream (`#F7F4EE`), Warm Stone (`#A39E99`), and Emerald Mint (`#10B981`).
- **Aesthetic Floating Glass Navigation Bar**:
  - Pure typographic wordmark: **DEFENDX** (no logo needed).
  - Segmented pill navigation with frosted glassmorphism (`backdrop-blur-2xl`).
  - Active indicator pills, subtle ambient glow, and warm pill action buttons.
- **Warm 3D Living Web Visualization**:
  - Procedural Three.js architectural web suspended in a warm ambient space.
  - Interconnected amber and champagne filaments with floating warm embers.
  - Interactive mouse parallax and real-time scanner wave pulses.

---

## ⚡ Core Features

1. **Multi-Vector Real Security Scanning**
   - **Secrets & Credentials**: Detects live Stripe API keys, AWS Access Key IDs, GitHub PATs, unencrypted private keys, and database connection strings.
   - **Evidence Masking**: Sensitive tokens are masked at the scanner kernel before rendering (e.g. `sk_live_51Ny*******************4819`).
   - **AST SAST Engine**: Identifies SQL injection (string formatting/concatenation), Command Injection (`subprocess(..., shell=True)`), DOM XSS (`dangerouslySetInnerHTML`), and Insecure Deserialization (`pickle.loads`).
   - **Web Endpoint Audit**: Probes TLS, HSTS, CSP, and Clickjacking (`X-Frame-Options`) headers.

2. **Interactive Threat Constellation**
   - Topological network map showing findings as interactive nodes connected to the project core. Click any node to open finding evidence.

3. **AI Remediation Studio**
   - Synthesizes 1-click copyable prompts formatted for Claude, ChatGPT, Cursor, and Copilot.
   - Generates code diff previews and verification checklists.
   - Real finding lifecycle tracking (`New` → `Reviewed` → `Repair Suggested` → `Needs Manual Verification` → `Eliminated`).

4. **Side-by-Side Rescan Diff Comparison**
   - Differential comparison tracking eliminated findings vs active issues with calculated improvement deltas (e.g. `+85% Security Posture Improvement`).

5. **Beginner Assistance Mode ("Explain Like I'm New")**
   - 1-click toggle translating technical CVEs into:
     - *What happened?*
     - *Why should I care?*
     - *What to change?*
     - *How to check the fix?*

6. **Instant Hackathon Demo Mode**
   - Pre-loaded with synthetic vulnerable and remediated payment gateway codebases (`ApexPay`) allowing judges to experience the entire workflow without external API keys.

---

## 🚀 Running the Application

### 1. Backend API (FastAPI)
```powershell
$env:PYTHONPATH="backend"
python -m uvicorn app.main:app --port 8000 --reload
```
API Documentation: `http://127.0.0.1:8000/docs`

### 2. Frontend (React + Vite)
```powershell
cd frontend
npm.cmd run dev
```
Application: `http://localhost:3000`

### 3. Run Test Suite
```powershell
$env:PYTHONPATH="backend"
python -m pytest backend/app/tests
```
