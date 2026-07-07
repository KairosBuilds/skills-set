# Examples — CLI Engineer

## Example: Todo CLI Tool
**Requirements:** CLI for managing todo items

**Design:**
- Commands: add, list, complete, delete
- Flags: --priority, --project, --due
- Output: formatted table, --json support

**Implementation (Go + Cobra):**
1. Root command with subcommands
2. todo add "Buy groceries" --priority high --project home
3. todo list --project home
4. todo complete 123
5. Shell completions for bash/zsh/fish
6. JSON output for scripting

**Output:** Complete todo CLI tool with shell completion