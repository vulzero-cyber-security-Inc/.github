<div align="center">

# VULZERO

**Authorized security research.** Scanners forget — Vulzero remembers.

[vulzero.cc](https://vulzero.cc) · [academy.vulzero.cc](https://academy.vulzero.cc) · contact@vulzero.cc

</div>

---

Vulzero Cybersecurity Inc. is a federally incorporated Canadian company (Corporation No. 1604585-5, Cambridge, Ontario) doing **authorized** penetration testing, vulnerability assessment, and bug-bounty coordination. The work happens inside an environment that keeps what each engagement learned and ties every conclusion to evidence — because a finding you cannot trace to evidence is a rumor with a severity rating, and we will not ship one.

Two people do the work, and the one who did it signs it: **Ammar Rahmouni** (assessments, end to end) and **Mohamed Ibrahim** (bug-bounty coordination). No bench, no rotating juniors, no subcontracting.

## How we work — four boundaries, enforced in code

- **Authorization first.** No work starts before a signed scope exists in the system, and every action is checked against it before it runs.
- **Evidence before conclusions.** Artefacts are hashed the moment they are captured and chained to the ones around them, so every conclusion resolves back to its proof in one step.
- **Human approval, enforced.** Anything consequential stops at a gate that records who said yes, and to what.
- **Never fabricate evidence.** A gap in the record is written down as a gap.

## What we build

Most of this is early — each project states plainly what runs today and what is still a plan.

| Project | What it is |
| --- | --- |
| **Vulzero Platform** | Policy, scope, evidence, audit and bounded-assistant services — the environment engagements run inside. |
| **Vulzero Evidence** | A portable `.vzb` bundle format: hash-chained events, an Ed25519-signed manifest and timestamps, verifiable offline without trusting the researcher. |
| **Vulzero Verify** | Self-hosted ASGI middleware that scores a request from its headers and can ask a suspicious browser to solve a proof-of-work challenge. |
| **VZL** | An experimental, dependency-free programming language in Rust: statically typed, compiled to verified bytecode, run on a fuel- and memory-bounded VM with no ambient authority. |
| **VZ-Scan** | A consent-gated, read-only exposure check: prove ownership, choose what to test and at what rate, get an encrypted, time-bound report. No exploit payloads. |
| **Vulzero Academy** | Offensive-security training — penetration testing, exploit development, red-team operations and more, with real labs and CTF challenges. |

## Try the tools, in your browser

The developer pages run the real tools client-side, nothing uploaded:

- **[Scope resolver](https://vulzero.cc/developers)** — the real `@vulzero/scope`: allow/deny with exclusion-first dominance.
- **[Verify scorer + proof-of-work](https://vulzero.cc/developers/verify)** — the real passive scorer and SHA-256 PoW.
- **[Evidence verifier](https://vulzero.cc/developers/evidence)** — build and verify a hash-chained, signed `.vzb` bundle; tamper it and watch it break.
- **[VZL playground](https://vulzero.cc/developers/vzl)** — the real compiler and VM, compiled to WebAssembly.

## Work with us

- **Scope an engagement** — authorized assessment, research retainer, or bug-bounty coordination: contact@vulzero.cc
- **Report a vulnerability** in our own systems: security@vulzero.cc · [`/.well-known/security.txt`](https://vulzero.cc/.well-known/security.txt)
- **Researchers** — a small, vetted pool works our authorized programs: research@vulzero.cc

<div align="center">
<sub>VULZERO CYBERSECURITY INC. · Authorized research only.</sub>
</div>
