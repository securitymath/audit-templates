# Audit Methodology

## 5-Phase Approach

### Phase 1: Scoping (Day 1)
- Define attack surface and critical invariants
- Review previous audits and known issues
- Identify external dependencies and trust assumptions

### Phase 2: Manual Review (Days 2-7)
- Line-by-line analysis of all in-scope contracts
- Focus areas: access control, arithmetic, reentrancy, oracle usage
- Document all assumptions and invariants

### Phase 3: Automated Analysis (Days 3-8)
- Slither + custom detectors
- Foundry fork tests for all critical paths
- Gas analysis for DoS vectors

### Phase 4: Formal Verification (Days 5-10)
- Halmos symbolic execution for critical invariants
- Echidna fuzzing for property-based testing
- Certora rules for complex state machines

### Phase 5: Reporting (Days 9-12)
- Finding writeup with PoC
- Severity assessment and prioritization
- Fix recommendations and verification plan
