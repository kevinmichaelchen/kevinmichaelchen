# CLAUDE.md

Project instructions for Claude Code.

## Adding New GitHub Projects

When adding a new GitHub repository to the README, gather information using:

1. **GitHub CLI for description**:
   ```bash
   gh repo view OWNER/REPO --json description -q '.description'
   ```

2. **GitHub CLI for README**:
   ```bash
   gh api repos/OWNER/REPO/readme --jq '.content' | base64 -d
   ```

Use the description for the table entry and consult the README for context on what emoji/category fits best.
