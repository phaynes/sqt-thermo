# SQT Paper Update Recovery Process

## CRITICAL: Recovery Instructions for Session Restart

### Context Minimization Strategy
This file contains everything needed to resume work without re-reading all original documents.

### Current Status: Attempt #6
**Last Updated**: 2025-06-04
**Current Transaction**: Setting up transaction system

### Recovery Steps for New Session:

1. **Read Only These Files**:
   - `/Volumes/second-store/devel/sqt-thermo/recovery-process.md` (this file)
   - `/Volumes/second-store/devel/sqt-thermo/current-paper-state.Rmd` (latest version)
   - `/Volumes/second-store/devel/sqt-thermo/current-transaction.md` (what to do next)

2. **Do NOT Re-read**:
   - Original papers (key issues already extracted below)
   - Review comments (already summarized below)
   - Prior drafts (superseded)

### Transaction-Based Update Plan

Each transaction is a single, focused change that:
- Takes < 5 minutes
- Updates one specific issue
- Saves result immediately
- Updates progress tracking

### Key Issues Summary (from reviews):

#### A. Scientific Accuracy Fixes Needed:
1. **A1**: Heat capacity correction has wrong dimensions. Need energy scale factor.
2. **A2**: First Law needs quasi-static assumption stated explicitly
3. **A3**: Second Law needs Spohn condition for non-unital channels
4. **A4**: Jarzynski coherence factor C[ρ₀,ρf] undefined
5. **A5**: Function f(ε) in info processing bound undefined
6. **A6**: Volume vs area in holographic section needs clarification
7. **A7**: ρ_coh (coherence energy density) undefined
8. **A8**: Code blocks have undefined variables (U_t, gamma)

#### B. Missing from v2:
- Experimental feasibility paragraph
- Spohn (1978) citation
- Notation/units subsection
- Testability table

#### C. Presentation:
- Theorem numbering resets
- Convert to third person throughout
- Fix LaTeX/references

#### D. Major Conceptual Issues:
- Division events need physical characterization
- Entropy jump contradiction at division events (Appendix A.2)
- Chronon τ scale needs clear definition

### Transaction Order:

**Phase 1: Critical Scientific Fixes (A1-A8)**
- T1: Fix heat capacity dimensions (A1)
- T2: Add quasi-static assumption (A2)
- T3: Add Spohn condition (A3)
- T4: Define coherence factor (A4)
- T5: Define f(ε) function (A5)
- T6: Fix volume/area issue (A6)
- T7: Define ρ_coh (A7)
- T8: Fix code variables (A8)

**Phase 2: Restore Missing Elements (B)**
- T9: Add experimental feasibility
- T10: Add Spohn citation
- T11: Add notation section
- T12: Add testability table

**Phase 3: Major Conceptual Fixes (D)**
- T13: Clarify division events
- T14: Fix entropy contradiction
- T15: Define chronon scale

**Phase 4: Third Person Conversion**
- T16-T20: Convert sections to third person

**Phase 5: Final Polish**
- T21: Fix theorem numbering
- T22: Fix references
- T23: Final review

### File Structure:
```
/Volumes/second-store/devel/sqt-thermo/
├── recovery-process.md          (this file - always read first)
├── current-paper-state.Rmd      (latest full paper)
├── current-transaction.md       (next step to do)
├── completed-transactions.log   (what's been done)
└── transaction-backups/         (backup after each transaction)
    ├── T1-complete.Rmd
    ├── T2-complete.Rmd
    └── ...
```

### Quick Reference Formulas (to avoid re-reading):

**Heat Capacity Correction** (needs dimension fix):
Currently: ħ²/(mτ²k_BT) - wrong dimensions
Should be: ħ²⟨(∇V)²⟩/(12mk_BT²τ²) or similar

**Entropy at Division Events** (contradiction to fix):
Main text says: ΔS_vN ≥ 0
Appendix A.2 says: ΔS_vN = -S_coh ≤ 0
Resolution: Need to clarify what happens to total vs coherence entropy

**Key SQT Equations**:
- Γᵢⱼ(t) = tr[Θ†(t)PᵢΘ(t)Pⱼ]
- ρ(t) = Θ(t)ρ(0)Θ†(t)
- S_coh = S_vN - S_stoch

### Next Action:
Read `/Volumes/second-store/devel/sqt-thermo/current-transaction.md` and execute that transaction only.
