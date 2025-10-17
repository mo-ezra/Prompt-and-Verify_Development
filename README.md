# Prompt-and-Verify Development (PaV)

**PaV** is an AI-assisted software method where engineers use natural-language prompts to generate code and **must** pass it through human review, automated tests, linters, and security checks before acceptance. Nothing merges without verification.

**Canonical page:** https://<your-username>.github.io/prompt-and-verify-development/

---

## Why PaV (vs. “vibe coding”)

| Aspect | Vibe coding | PaV |
| --- | --- | --- |
| Review depth | Minimal / opportunistic | **Mandatory, deep** |
| Quality gates | May skip or defer | **Tests, lint, security, CI required** |
| Risk posture | Prototype-first | **Reliability-first** |
| Suitable for | Fast prototyping | **Production & regulated teams** |

---

## Reference workflow

1. **Frame** — write/attach a brief spec or tests first.  
2. **Prompt** — ask the LLM for scoped, testable changes.  
3. **Build locally** — run unit tests, lints, type checks.  
4. **Review** — human code review; request fixes or hand-edit.  
5. **Gate** — CI must pass verification checks before merge.  
6. **Document** — commit prompts & decisions (ADR/changelog).

---

