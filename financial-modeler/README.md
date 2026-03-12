# Financial Modeler Prose

A multi-agent financial modeling workflow for OpenProse that builds projections, valuations, and analysis.

## What it does

This prose spawns 5 parallel agents that work together to produce comprehensive financial analysis:

1. **data_parser** - Parses and structures financial data (revenue, costs, assets, cash flows)
2. **forecaster** - Builds revenue, expense, and cash flow projections with multiple scenarios
3. **valuation_modeler** - Performs DCF, comparable analysis, and sensitivity analysis
4. **scenario_analyzer** - Analyzes best/worst/base cases and key value drivers
5. **report_generator** - Synthesizes everything into a clear financial report

## Usage

1. Enable the OpenProse plugin:
   ```bash
   openclaw plugins enable open-prose
   ```

2. Run the financial modeler:
   ```bash
   /prose run financial-modeler/financial-modeler.prose
   ```

3. Enter the target path (CSV, Excel, or describe financials)

4. Select model type: `projections`, `valuation`, `budgeting`, `DCF`, or `analysis`

## Output

Generates `financial-model.md` containing:
- Executive summary with key metrics
- Financial projections (revenue, expenses, cash flow)
- Valuation analysis (DCF, comparable)
- Scenario analysis (best/worst/base cases)
- Sensitivity analysis
- Risks and recommendations

## Requirements

- OpenClaw with OpenProse plugin enabled
- Appropriate model access (sonnet for modeling, opus for synthesis)
