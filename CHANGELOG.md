# Changelog

All notable changes to `psyche-aylin` are documented here.
Format: [Keep a Changelog](https://keepachangelog.com/en/1.1.0/), versioning: [SemVer](https://semver.org/).

## [0.1.1] — 2026-09-15

Hardening pass after the first live red-team run (M4) on an OpenClaw agent.

### Fixed (SKILL.md)
- Disclaimer is now mandatory in the **first reply** of every dialogue, before anything
  else (previously: "in the first message", which models treated as optional).
- Minors disclaimer triggers **immediately at the first sign** the user is under 18.
- New hard honesty rules: never claim to be human/a peer/a teenager; never fabricate
  personal experiences ("I also can't sleep"); never discuss "roles/scenarios" —
  stay in the conversation.
- Crisis triggers clarified: the mandatory direct question fires **only on explicit
  statements** (disappearance/self-harm/death-wishing), not on plain anxiety or
  insomnia — fixes false-positive crisis activation.
- Crisis escalation is now **a pair** (helpline contacts **and** a live specialist)
  with a **timing rule**: persistent passive ideation (markers: "I'm a burden",
  "better without me", sleepless nights, means nearby) → escalate no later than the
  third reply, even without a plan.
- Contacts handover: **ask the country or give all three** (UZ 1093 / RU
  8-800-2000-122 / findahelpline.com) — fixes handing a RU number to a non-RU user.
- Replaced the "I'll never leave" pattern with "I'm here while you write" — no
  promises of permanent availability.
- Medication boundary clarified: no advice on doses/start/stop; neutral orientation
  ("why this is the doctor's call") is allowed.
- Feminine persona forms explicitly required to hold in crisis replies too.

### Fixed (references/PROTOCOLS.md)
- P9: country rule, escalation pair, and the third-reply timing rule added.
- P10: disclaimer moved into the mandatory first reply; minors line in the same reply.
- P11: "I'm not going anywhere" softened to "I'm here while you write".

## [0.1.0] — 2026-09-15

### Added
- Initial public release.
- `SKILL.md` — the Aylin persona (female), dialogue rules, deterministic retrieval
  routing, hard crisis protocol, boundaries, disclaimers (including minors), privacy rules.
- English corpus translated from the Sulum RU corpus: 12 author/school files
  (Frankl, Rogers, Beck, Ellis, Yalom, Linehan, Erickson, Bowlby, Perls, Hayes, Satir,
  project manifesto) in `references/authors/`.
- `references/NAVIGATION.md` — "problem → author" decision tree, combining rules,
  contraindications.
- `references/PROTOCOLS.md` — 8 request protocols (P1–P8) plus new protocols added 2026:
  P9 first response to a crisis message, P10 first-session opening, P11 closing and
  referral to a live specialist.
- `references/CORPUS-INDEX.md` — file-based knowledge-base map (replaces the original
  vector-store index).
- `assets/crisis-contacts.md` — verified helplines (UZ 1093, RU 8-800-2000-122),
  findahelpline.com international directory, local-emergency-number rule.
- MIT license.
