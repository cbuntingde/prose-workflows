# Security Reviewer Prose

A multi-agent security review workflow for OpenProse that comprehensively scans code for vulnerabilities.

## What it does

This prose spawns 5 parallel agents that work together to produce a thorough security assessment:

1. **scanner** - Detects OWASP Top 10 vulnerabilities (SQL injection, XSS, command injection, etc.)
2. **dependency_auditor** - Checks dependencies for known CVEs and outdated packages
3. **secrets_detector** - Finds exposed API keys, tokens, passwords, and credentials
4. **architecture_reviewer** - Evaluates security patterns and provides recommendations
5. **report_synthesizer** - Merges all findings into a prioritized markdown report

## Usage

1. Enable the OpenProse plugin:
   ```bash
   openclaw plugins enable open-prose
   ```

2. Run the security reviewer:
   ```bash
   /prose run security-reviewer/security-reviewer.prose
   ```

3. Enter the target path when prompted (file or directory)

4. Select scope: `full`, `quick`, or `critical-only`

5. Results are saved to `security-review.md` in your workspace

## Output

Generates `security-review.md` containing:
- Executive summary
- Critical and high-severity findings with file/line references
- Dependency vulnerabilities (CVEs)
- Exposed secrets locations
- Architecture recommendations

## Requirements

- OpenClaw with OpenProse plugin enabled
- Appropriate model access (sonnet for scanning, opus for synthesis)
