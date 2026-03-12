# Contract Reviewer Prose

A multi-agent contract analysis workflow for OpenProse that reviews contracts for risks and problematic clauses.

## What it does

This prose spawns 5 parallel agents that work together to produce a comprehensive contract review:

1. **clause_extractor** - Catalogues all significant clauses (parties, dates, obligations, termination, liability, etc.)
2. **risk_analyzer** - Identifies legal/business risks (unlimited liability, vague language, one-sided terms)
3. **comparison_agent** - Compares against industry standard clauses for the contract type
4. **summary_writer** - Synthesizes findings into a clear, plain-language summary
5. **negotiator** - Provides specific recommended changes and negotiation points

## Usage

1. Enable the OpenProse plugin:
   ```bash
   openclaw plugins enable open-prose
   ```

2. Run the contract reviewer:
   ```bash
   /prose run contract-reviewer/contract-reviewer.prose
   ```

3. Enter the target path when prompted (PDF, DOCX, or text file)

4. Select contract type: `generic`, `NDA`, `employment`, `service`, `lease`, or `other`

## Output

Generates 4 files:
- `contract-clauses.md` - Extracted clauses with locations
- `contract-risks.md` - Risk analysis with severity ratings
- `contract-summary.md` - Plain-language summary
- `contract-negotiations.md` - Specific recommendations for negotiation

## Requirements

- OpenClaw with OpenProse plugin enabled
- Appropriate model access (sonnet for extraction/analysis, opus for synthesis)
