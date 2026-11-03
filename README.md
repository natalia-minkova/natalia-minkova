# Natalia Minkova — Cyber Kimura

**Authority security for autonomous systems — AI agents, drones & robots.**

I test who can command a system, which actions they can authorize, and whether those limits hold after replay, reconnects and software changes.

**[Read the A02 case study](https://cyberkimura.com/case-study/) · [Run the public lab](https://github.com/natalia-minkova/authority-replay-lab) · [Contact me](mailto:security@cyberkimura.com)**

> A claim isn't proof. Review the test conditions, observed results and limits;
> run the public lab to check its assertions yourself.

---

### Focus
`authority & command security` · `AI / LLM agents` · `drone / UAS command links` · `robot actuators` · `red team`

### Selected work
- **Authority Replay (A02)** — a consumed authorization cannot be replayed; enforcement
  confirmed by mutation testing, evidence reproduced from a clean environment.
  *(synthetic, software-only)* → [case study](https://cyberkimura.com/case-study/)
- **Drone command-link security** — an unsigned ground-station command was accepted,
  then rejected after enabling MAVLink2 signing; includes a trust-boundary finding.
  *(ArduPilot SITL; dedicated report and reproduction package not yet published.)*

### Public code — start here

**[Authority Replay Lab](https://github.com/natalia-minkova/authority-replay-lab)** — a standalone Python/SQLite example with 11 tests, concurrent replay checks, transaction rollback and a targeted mutation check. No dependencies beyond the Python standard library.

Run it locally: `python3 -m unittest -v` and `python3 check_mutation.py`.

This educational lab illustrates the single-use-authority principle; it is not the A02 source release or a reproduction of its historical results. Proprietary assessment tooling, fuzzing strategies and client artifacts remain private.

### Method — Authority Continuity Assessment
Authority · link-loss & reconnect · persistence after change · result vs claim ·
reproducible proof. One approach across agents, drones and robots.

### Stack
Python · ArduPilot / MAVLink · RTL-SDR · pytest · reproducible test harnesses

---

🌐 cyberkimura.com · ✉️ security@cyberkimura.com · Amsterdam · open to remote
