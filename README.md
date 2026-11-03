# Natalia Minkova — Cyber Kimura

**Offensive security for systems that take real-world actions — AI agents, drones, robots.**

I test whether a system actually enforces *who is allowed to command it* — and investigate whether those boundaries hold after link loss, reconnects, and changes to code, configuration or environment.

> A claim isn't proof. My approach centres on versioned test conditions, parameters, logs and reproducible results.

---

### Focus
`authority & command security` · `AI / LLM agents` · `drone / UAS command links` · `robot actuators` · `red team`

### Selected work
- **Authority Replay (A02)** — replay of a consumed authorization was rejected in the tested scenarios; enforcement checked through mutation testing and results reproduced from a clean environment. *(Synthetic, software-only)* → [Case study](https://cyberkimura.com/case-study/)
- **Drone command-link security** — an unsigned ground-station command was accepted in the initial configuration, then rejected on the protected command link after enabling MAVLink 2 signing; testing also identified a trust-boundary issue involving a trusted station. *(ArduPilot SITL; no real aircraft)*
- **Client AI-agent assessment** — a high-severity authority-related finding identified during a client engagement. *(Details under NDA)*

### Method — Authority Continuity Assessment
Authority · link loss & reconnect · persistence after change · reported result vs observed outcome · reproducible evidence.

One approach across agents, drones and robots, with conclusions bounded by the configuration and scenarios tested.

### Stack
Python · ArduPilot / MAVLink · RTL-SDR · pytest · signed evidence capsules

---

🌐 [cyberkimura.com](https://cyberkimura.com) · ✉️ [security@cyberkimura.com](mailto:security@cyberkimura.com) · Amsterdam · Open to remote engagements
