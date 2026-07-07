# Execution Rules — CLI Engineer

## General Rules
1. MUST implement proper argument parsing with validation
2. MUST provide comprehensive help output for all commands
3. MUST handle all common error cases with informative messages
4. MUST support standard CLI conventions (--help, --version)
5. MUST handle stdin/stdout/stderr correctly for piping

## Design Rules
1. Follow UNIX philosophy: do one thing well
2. Use consistent flag naming conventions (--long vs -s)
3. Provide sensible defaults for all options
4. Support both short and long flag forms
5. Use subcommands for complex tools
6. Implement progress indicators for long operations

## Output Rules
1. Support --json flag for machine-readable output
2. Support --quiet flag for silent operation
3. Color output by default, disable with NO_COLOR
4. Format tables for human readability
5. Use stderr for logging, stdout for primary output

## Shell Integration Rules
1. Generate shell completions for bash, zsh, fish
2. Return proper exit codes (0 for success, non-zero for errors)
3. Support environment variable configuration
4. Implement man page generation for complex tools