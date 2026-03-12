# Patent Landscaper Prose

A multi-agent workflow for OpenProse that analyzes patent landscapes, trends, and IP positioning.

## What it does

This prose spawns 5 parallel agents that work together to produce a comprehensive patent landscape analysis:

1. **patent_searcher** - Searches for patents, identifies key patents and major assignees
2. **trend_analyzer** - Analyzes filing trends, growth areas, and temporal patterns
3. **competitor_analyzer** - Analyzes key players' patent portfolios and IP strategies
4. **gap_identifier** - Identifies white spaces, underserved areas, and opportunities
5. **landscape_reporter** - Synthesizes everything into a strategic IP report

## Usage

1. Enable the OpenProse plugin:
   ```bash
   openclaw plugins enable open-prose
   ```

2. Run the patent landscaper:
   ```bash
   /prose run patent-landscaper/patent-landscaper.prose
   ```

3. Enter the technology or industry to analyze

4. Select focus: `analysis`, `search`, `validation`, or `competitive`

## Output

Generates `patent-landscape.md` containing:
- Executive summary
- Key patents and assignees
- Filing trends and growth patterns
- Competitive landscape
- White space opportunities
- Strategic IP recommendations

## Use cases

- R&D portfolio planning
- Freedom to operate analysis
- Competitive intelligence
- Investment due diligence
- M&A target evaluation

## Requirements

- OpenClaw with OpenProse plugin enabled
- Appropriate model access (sonnet for search/analysis, opus for synthesis)
