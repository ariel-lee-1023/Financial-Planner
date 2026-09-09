# Changelog

All notable changes to this skill are documented here.

The format follows [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased] — Expert core and project guidance

- Rewrote the master as a first-person planner whose judgments connect cash-flow timing, debt, liquidity, and life-stage utility.
- Moved detailed framework lookup behind task triggers and clarified that source thresholds require household-specific interpretation.
- Added root `AGENTS.md` for default skill loading and repository work.

## [1.1.0] — 2026-08-07

### Changed
- **Lengthened all four book references and the synthesis** to study-depth density using the latest Books-to-Skill-Refs extraction discipline (structure over summary, author terminology, Mental Model → Frameworks by section → Worked Example → Decision Rules & Judgment → Key Takeaways).
- `references/die-with-zero.md` — expanded from short summary to full nine-rule structural distillation with memory dividend, personal interest rate, survival threshold formula, time-bucketing, net-worth peak, and asymmetric-risk rule.
- `references/value-of-debt.md` — expanded debt taxonomy table, L.I.F.E. glide-path phases, D/A bands by net-worth-to-income, securities-based lending 25% guardrail, three money buckets, and appendices (SBL, home financing, millennial guide).
- `references/corporate-finance.md` — expanded NPV/opportunity-cost core, after-tax WACC, real-options justification for liquidity, household translation of capital-structure theory, and applicability limits.
- `references/financial-planning-process.md` — expanded seven-step process, foundation hierarchy, behavioral/suitability overlay, wills/trusts/fiduciaries notes, and CFP alignment.
- `references/synthesis-and-examples.md` — expanded six-gate decision tree, three fully worked examples (degree sequencing, mortgage vs. windfall, early-career bold move), and synthesizer decision rules.

### Distillation notes
- Sources: full extracted text of Perkins *Die with Zero*, Anderson *The Value of Debt in Building Wealth*, Brealey et al. *Principles of Corporate Finance* (14th), and front-matter/structure of Leimberg *Tools & Techniques of Financial Planning* (12th).
- Method: Books-to-Skill-Refs (https://github.com/ariel-lee-1023/Books-to-Skill-Refs) study-depth template; never raw-copied; density over length; exact framework names preserved.

## [1.0.1] — 2026-08-07

### Changed
- Renamed persona and skill id from **Seasoned Financier** / `seasoned-financier` to **Financial Planner** / `financial-planner` across `SKILL.md`, `README.md`, and reference text.

## [1.0.0] — 2026-08-07

### Added
- Core `SKILL.md` — Financial Planner persona, four-framework decision tree (Gates 1–6), operating procedure, clarifying-question defaults, and output shape
- `references/value-of-debt.md` — Anderson (*The Value of Debt in Building Wealth*): debt taxonomy, after-tax return equivalence, liquidity, glide-path D/A ratios
- `references/corporate-finance.md` — Brealey/Myers/Allen (*Principles of Corporate Finance*): NPV, opportunity cost of capital, after-tax cost of debt, WACC
- `references/financial-planning-process.md` — Leimberg et al. (*Tools & Techniques of Financial Planning*): cash-flow planning, seven-step process, foundation-first hierarchy
- `references/die-with-zero.md` — Perkins (*Die with Zero*): nine rules, memory dividend, personal interest rate, survival threshold, net-worth peak
- `references/synthesis-and-examples.md` — cross-book conflict resolution and two fully worked examples (multi-goal degree funding; low-rate mortgage vs. windfall)
- Standard packaging: README, LICENSE (MIT), NOTICE, CHANGELOG, .gitignore

### Distillation notes
- Built as a multi-source skill library (Books-to-Skill-Refs pattern). Structure over summary; authors' exact framework names and decision rules preserved; applicability limits stated explicitly for each source.
- Unified decision tree resolves Anderson/Perkins and pure-NPV/utility conflicts by client position relative to foundation line and survival threshold.
