# audit-templates

Standardized audit report templates and security review checklists used by Security Math.

## Contents

- `checklist/` — Pre-audit and post-audit checklists
- `templates/` — Methodology, severity classification, report structure

## Audit Methodology

Our review process follows a 5-phase approach:

1. **Scoping** — Define attack surface, identify critical invariants
2. **Manual review** — Line-by-line analysis of all in-scope contracts
3. **Automated analysis** — Slither, custom detectors, Foundry fork tests
4. **Formal verification** — Halmos/Echidna for critical properties
5. **Reporting** — Findings with PoC, severity rating, and fix recommendations

See `templates/methodology.md` for detailed breakdown.

## Severity Classification

| Severity | Description |
|----------|-------------|
| Critical | Direct fund loss or permanent DoS without user interaction |
| High | Conditional fund loss or significant protocol disruption |
| Medium | Indirect fund loss, governance manipulation, or limited impact |
| Low | Best practice violations, gas optimizations, code clarity |

See `templates/severity.md` for full guide.

## License

Internal use. Public for reference only.
