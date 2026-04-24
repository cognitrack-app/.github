# CogniTrack

> **Know Your Brain. Own Your Focus.**  
> Real-time cognitive load monitoring — built for knowledge workers.

CogniTrack tracks context switches, attention residue, and cognitive debt across your workday, then surfaces actionable recovery protocols before burnout hits.

---

## How It Works

```
macOS Menu Bar App  ──▶  Local SQLite  ──▶  Sync Engine  ──▶  Firebase
      │                                                            │
      └──────────────────────────────────────────────────────────▶│
                                                                   ▼
                                                         Cognitive Engine
                                                     (debt · residue · recovery)
                                                                   │
                                                                   ▼
                                                          Mobile Dashboard
                                                    (iOS · Android — coming soon)
```

1. **Desktop agent** tracks active window switches passively in the background
2. **Cognitive engine** converts raw switches into Cognitive Debt, Attention Residue, and Focus Blocks
3. **Firebase backend** stores derivations, runs scheduled rollups, and serves the mobile app
4. **Mobile app** surfaces your Daily Brain Load, Weekly Patterns, and personalised Recovery Plans

---

## Repositories

| Repo | Description | Status |
|---|---|---|
| [cognitrack-backend](https://github.com/cognitrack-app/cognitrack-backend) | Firebase Functions · Firestore · Shared packages | 🟢 Active |
| [cognitrack-desktop](https://github.com/cognitrack-app/cognitrack-desktop) | Electron + React · macOS tray agent | 🟢 Active |
| [cognitrack-mobile](https://github.com/cognitrack-app/cognitrack-mobile) | Flutter · iOS + Android dashboard | 🔵 Planned |
| [cognitrack-docs](https://github.com/cognitrack-app/cognitrack-docs) | Architecture docs · API reference | 🔵 Planned |

---

## Core Metrics

| Metric | What It Measures |
|---|---|
| **Cognitive Debt** | Accumulated mental load from unrecovered context switches |
| **Switch Velocity** | Context switches per hour vs. your personal baseline |
| **Attention Residue** | Carry-over cognitive load between tasks |
| **Focus Blocks** | Uninterrupted deep work windows |
| **Recovery Coefficient** | Efficiency gain after structured breaks |
| **Readiness Score** | Predicted next-day cognitive baseline |

---

## Tech Stack

```
Desktop     Electron · React · TypeScript · SQLite · Vite
Backend     Firebase Functions · Firestore · TypeScript
Mobile      Flutter (planned)
Shared      pnpm workspaces · packages/shared · packages/sync-engine
```

---

## Status

Currently in **private alpha** — desktop agent + backend fully functional.  
Mobile dashboard in design phase.

---

*Built by [@MUGEN1603](https://github.com/MUGEN1603)*
