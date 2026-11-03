# Natalia Minkova — Cyber Kimura

**Offensive security for systems that take real-world actions — AI agents, drones, robots.**

I test the one thing most teams never verify: whether a system actually enforces
*who is allowed to command it* — and whether that holds after link loss, reconnects,
and changes to code, config or environment.

> A claim isn't proof. Every finding ships with the version, parameters, logs,
> and a result you can re-run.

---

### Focus
`authority & command security` · `AI / LLM agents` · `drone / UAS command links` · `robot actuators` · `red team`

### Selected work
- **Authority Replay (A02)** — a consumed authorization cannot be replayed; enforcement
  confirmed by mutation testing, evidence reproduced from a clean environment.
  *(synthetic, software-only)* → [case study](https://cyberkimura.com/case-study/)
- **Drone command-link security** — an unsigned ground-station command was accepted,
  then rejected after enabling MAVLink2 signing; includes a trust-boundary finding.
  *(ArduPilot SITL)* → [website](https://cyberkimura.com)
- **Production AI-agent assessment** — high-severity authority flaw found in a client
  engagement. *(details under NDA)*

### Public code — start here

**[Authority Replay Lab](https://github.com/natalia-minkova/authority-replay-lab)** — a standalone Python/SQLite example with 11 tests, concurrent replay checks, transaction rollback and a targeted mutation check. No dependencies beyond the Python standard library.

Run it locally: `python3 -m unittest -v` and `python3 check_mutation.py`.

This educational lab illustrates the single-use-authority principle; it is not the A02 source release or a reproduction of its historical results. Proprietary assessment tooling, fuzzing strategies and client artifacts remain private.

### Method — Authority Continuity Assessment
Authority · link-loss & reconnect · persistence after change · result vs claim ·
reproducible proof. One approach across agents, drones and robots.

### Stack
Python · ArduPilot / MAVLink · RTL-SDR · pytest · signed reproducible evidence

---

🌐 cyberkimura.com · ✉️ security@cyberkimura.com · Amsterdam · open to remote
