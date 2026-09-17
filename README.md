# Financial Planner

I help you decide what money should do next by putting the dates back into the calculation. I trace when income arrives, when obligations fall due, which goals are committed, and what remains accessible if a plan goes wrong. Education, a home, retirement, and a business can draw on the same assets at different times. A choice that looks attractive in isolation may leave the next commitment unfunded.

If you ask whether to repay a loan or invest the cash, I compare the actual payment and reserve paths. Avoided borrowing costs and uncertain investment returns need a consistent after-tax, risk-aware comparison. I then test an income interruption, a rate reset, or a fall in asset values. A modest expected advantage carries less weight if it forces a sale or consumes the money already needed for tuition. I classify a debt by its terms and effect on the household, and explain the condition that would make repayment or retention preferable.

I also ask what the money is for. An experience with a real life-stage window may justify spending that a balance-sheet-only comparison would postpone. That judgment still has to accommodate dependants, longevity uncertainty, intended gifts, and your own margin for comfort. I give you a recommended course, the assumptions carrying it, and the observable change that would warrant revisiting it.

This Agent Skill draws on four financial frameworks and a synthesis module, connecting timed cash flows, liquidity, opportunity cost, and the changing usefulness of wealth.

## Layout

```
SKILL.md                              # expert reasoning core + task-based loading triggers (always loaded)
references/
  value-of-debt.md                    # Anderson — debt taxonomy, glide-path, liquidity
  corporate-finance.md                # Brealey/Myers/Allen — NPV, opportunity cost, WACC
  financial-planning-process.md       # Leimberg — cash-flow planning, 7 steps, foundation-first
  die-with-zero.md                    # Perkins — lifetime fulfillment, personal interest rate
  synthesis-and-examples.md           # conflict resolution + worked examples
```

`SKILL.md` is the expert entrypoint; root `AGENTS.md` also guides work when this repository is opened as a project. It sets the planner’s judgment and interaction style, then routes to references only when the question needs their depth.

## Sources

| Source | Role in the skill |
|---|---|
| **The Value of Debt in Building Wealth** — Thomas J. Anderson | Debt taxonomy, after-tax return equivalence, liquidity as insurance, glide-path D/A ratios by net-worth-to-income |
| **Principles of Corporate Finance** — Brealey, Myers & Allen | NPV rule, opportunity cost of capital, after-tax cost of debt, WACC (the neutral arithmetic layer) |
| **The Tools & Techniques of Financial Planning** — Leimberg et al. | Cash-flow planning as the outer loop, seven-step process, household-specific emergency liquidity and catastrophic-risk protection as constraints on optimization |
| **Die with Zero** — Bill Perkins | Objective function = lifetime fulfillment; memory dividend; age-rising personal interest rate; survival threshold; net-worth peak |

## What it does

| Capability | What you get |
|---|---|
| **Debt-vs-cash tradeoffs** | Classifies the debt first, computes the after-tax spread, and only then recommends pay-down, keep, or restructure |
| **Multi-goal sequencing** | Treats the problem as cash-flow timing; runs a liquidity stress test that sits *above* raw NPV so one goal cannot strand another |
| **Leverage sizing** | Source glide-path heuristics evaluated against actual debt service, liquidity, and downside scenarios |
| **Life-stage utility** | Once foundation and survival threshold are clear, applies Perkins' rising personal interest rate to age-locked experiences |
| **Explicit sensitivity** | Material assumptions and the conditions that could change the recommendation; quantify them when the inputs support it |

## Install

Clone the complete repository, then place it in your host's configured skill directory:

```bash
git clone https://github.com/ariel-lee-1023/Financial-Planner.git financial-planner
```

Keep the complete `SKILL.md` and `references/` tree together. Match the installed folder name to the `name:` field in `SKILL.md`.

## Usage

Ask normally; the skill triggers on personal-finance decision questions of the form "should I pay cash or borrow", "pay off the loan or invest", "fund goal A without stranding goal B", refinance / restructure, retirement drawdown sequencing, etc.

For a debt-versus-cash comparison, a useful answer might follow this sequence; adapt it to the question:

> Recommendation → debt classification + after-tax comparison → liquidity / stress check → assumptions and sensitivity note ("this flips if …").

It asks for missing facts that change the decision and can make conditional progress with explicitly stated assumptions. Source thresholds are heuristics, not universal current limits.

## What kind of distillation this is

Structure, not summary. Each reference file preserves the authors' own framework names and exact formulations, defines key terms inline, and ends with explicit **when it applies / does not** limits so the agent does not over-apply a book outside its stated domain. Nothing is copied verbatim at length; everything is synthesized for decision use.

## Scope and limitations

Strong on debt classification, after-tax cost-of-capital arithmetic, multi-goal liquidity, foundation-first ordering, and life-stage utility tradeoffs.

Out of scope by design: tax-return preparation, securities picking, single-objective factual lookups, and anything that requires a licensed advisor's signature. The skill is instructed to say so when the stakes warrant.

## Provenance

Built in the multi-source skill-library pattern (see [Books-to-Skill-Refs](https://github.com/ariel-lee-1023/Books-to-Skill-Refs)). The four source books remain the property of their respective rights holders; the reference files are structural distillations only.

## License

[MIT](LICENSE) — covering the original work here: the skill structure, expert core, loading guidance, README, and the distillation text as written.

The underlying books keep their own terms and are not relicensed by this. See [NOTICE.md](NOTICE.md).
