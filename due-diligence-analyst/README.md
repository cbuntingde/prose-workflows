# Due Diligence Analyst Prose

A multi-agent workflow for OpenProse that conducts comprehensive due diligence on companies, investments, or acquisitions.

## What it does

This prose spawns 7 parallel agents that work together to produce a thorough due diligence report:

1. **company_researcher** - Researches company overview, history, ownership, management
2. **financial_analyzer** - Analyzes financial health, revenue, profitability, cash flow
3. **market_analyzer** - Analyzes market position, competitive landscape, growth potential
4. **legal_compliance** - Reviews litigation, regulatory issues, IP, contracts
5. **risk_assessor** - Assesses operational, financial, market, and technology risks
6. **opportunity_evaluator** - Evaluates synergies, strategic value, and upside potential
7. **dd_reporter** - Synthesizes everything into a comprehensive report

## Usage

1. Enable the OpenProse plugin:
   ```bash
   openclaw plugins enable open-prose
   ```

2. Run the due diligence analyst:
   ```bash
   /prose run due-diligence-analyst/due-diligence-analyst.prose
   ```

3. Enter the company or investment target to analyze

4. Select type: `acquisition`, `investment`, `partnership`, or `vendor`

## Output

Generates `due-diligence.md` containing:
- Executive summary
- Company overview and history
- Financial analysis and health
- Market position and competitive landscape
- Legal and compliance review
- Risk assessment with ratings
- Opportunities and synergies
- Recommendations and conclusion

## Use cases

- M&A target evaluation
- Investment decisions
- Vendor assessment
- Partnership evaluation
- Investor due diligence

## Requirements

- OpenClaw with OpenProse plugin enabled
- Appropriate model access (sonnet for analysis, opus for synthesis)
