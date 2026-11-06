# CyberGuard 🛡️

Quantify cyber risk. Block compromise paths.

An interactive cybersecurity risk assessment platform that translates personal security habits into quantifiable scores. Simulate exploit chains, test real-time What-If mitigations, and compile security audit reports on a sleek interactive dashboard.

## Features

### 🔍 Security Assessment
- **Guided questionnaire** across multiple security categories
- **CIA scoring** (Confidentiality, Integrity, Availability) per answer
- **Risk levels**: Low → Medium → High → Critical
- **Progress tracking** with question navigation

### 🎯 What-If Analysis
Real-time mitigation impact simulation:
- Enable MFA
- Install antivirus
- Update OS
- Use unique passwords
- Secure WiFi

### 📊 Interactive Dashboard
- **Risk score visualization** with animated gauge
- **CIA triad breakdown** with radial charts
- **Attack path mapping** — visualize exploit chains
- **Mitigation recommendations** prioritized by risk reduction

### 🖥️ Sandbox Terminal
- Interactive command-line interface
- Simulated security tool outputs
- Learning-focused exploration

### 📄 Report Generation
- PDF/HTML export of assessment results
- Detailed findings with CIA impact
- Actionable remediation steps

## Tech Stack

| Layer | Technology |
|-------|------------|
| **Framework** | Next.js 15 (App Router) |
| **Language** | TypeScript (strict) |
| **Styling** | Tailwind CSS + CSS Variables |
| **State** | Zustand |
| **Icons** | Lucide React |
| **Charts** | Custom SVG/Canvas |
| **Deployment** | Vercel |

## Quick Start

```bash
# Install dependencies
npm install

# Run development server
npm run dev
```

Open [http://localhost:3000](http://localhost:3000).

## Project Structure

```
src/
├── app/
│   ├── assessment/     # Security questionnaire flow
│   ├── dashboard/      # Risk visualization & What-If
│   ├── reports/        # Report generation & export
│   ├── terminal/       # Sandbox terminal
│   ├── about-developer/ # Author info
│   ├── about-project/   # Project documentation
│   ├── layout.tsx      # Root layout
│   ├── page.tsx        # Landing page
│   └── globals.css     # Global styles
├── components/
│   └── layout/         # Shared layout components
├── stores/
│   └── assessment-store.ts  # Zustand store
├── types/
│   └── index.ts        # TypeScript definitions
└── lib/                # Utilities
```

## Key Concepts

### CIA Triad Scoring
Each answer impacts three dimensions:
- **Confidentiality** — Data privacy & access control
- **Integrity** — Data accuracy & tamper resistance
- **Availability** — System uptime & resilience

### Risk Levels
| Score | Level | Color |
|-------|-------|-------|
| 0–25 | Low | Green |
| 26–50 | Medium | Yellow |
| 51–75 | High | Orange |
| 76–100 | Critical | Red |

### What-If Toggles
Each mitigation shows real-time risk reduction:
```
Base Risk: 78 (High)
┌─ Enable MFA          → -22 points → 56 (Medium)
├─ Install Antivirus   → -15 points → 63 (Medium)
├─ Update OS           → -18 points → 60 (Medium)
├─ Unique Passwords    → -12 points → 66 (Medium)
└─ Secure WiFi         → -8 points  → 70 (High)
```

## Scripts

```bash
npm run dev       # Development server
npm run build     # Production build
npm run start     # Production server
npm run lint      # ESLint check
```

## Deploy on Vercel

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https%3A%2F%2Fgithub.com%2FAniket-Solanki%2FCyberGuard)

---

*Built with ❤️ by [Aniket Solanki](https://github.com/Aniket-Solanki)*
