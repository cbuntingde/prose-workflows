# Board Pack Assembler Prose

A multi-agent workflow for OpenProse that assembles board meeting materials into a cohesive pack.

## What it does

This prose spawns 5 parallel agents that work together to produce a complete board pack:

1. **document_collector** - Catalogs all source documents (financials, reports, appendices)
2. **financial_summarizer** - Summarizes financial statements, metrics, and variances
3. **operational_summarizer** - Summarizes KPIs, projects, and operational highlights
4. **strategic_summarizer** - Summarizes strategic progress and market position
5. **pack_assembler** - Assembles everything into a formatted board pack

## Usage

1. Enable the OpenProse plugin:
   ```bash
   openclaw plugins enable open-prose
   ```

2. Run the board pack assembler:
   ```bash
   /prose run board-pack-assembler/board-pack-assembler.prose
   ```

3. Enter the target folder path containing board documents

4. Select meeting type: `quarterly`, `annual`, `ad-hoc`, or `strategic`

5. Select audience: `board`, `executives`, `investors`, or `regulators`

## Output

Generates `board-pack.md` containing:
- Agenda
- Executive summary
- Financial review
- Operational review
- Strategic update
- Risk summary
- Decisions required
- Appendices reference

## Requirements

- OpenClaw with OpenProse plugin enabled
- Appropriate model access (sonnet for summarization, opus for assembly)
- Source documents in the target folder (PDFs, spreadsheets, text)
