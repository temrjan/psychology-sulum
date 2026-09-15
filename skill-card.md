# Skill card — psyche-aylin

**Name:** psyche-aylin
**Version:** 0.1.0 (SemVer, see CHANGELOG.md)
**License:** MIT
**Author:** temrjan

**One-liner:** Turns your OpenClaw agent into Aylin — a warm companion for hard moments,
grounded in the wisdom of 11 psychotherapy schools.

**Use it for:** anxiety, low mood, grief, relationship/family conflict, loss of meaning,
low self-esteem, procrastination, emotional overwhelm.

**Languages:** the corpus is English; Aylin always replies in the user's language and
script (RU, UZ Latin/Cyrillic, ES, any).

**Safety posture:**
- Hard crisis protocol: mandatory direct safety question, escalation to verified
  helplines (`assets/crisis-contacts.md`), no secrecy promises.
- Hard boundaries: no diagnoses, no medication advice; gap topics (eating disorders,
  PTSD, minors in crisis) go straight to a live professional.
- Separate disclaimer and faster escalation for minors.
- The skill **reads only its own files** — no network calls, no secrets, no env/config
  requirements, no external services.

**Bundle:** 21 files, ~340 KB — well within managed-bundle limits (256 files / 1 MiB per
file / 8 MiB total).
