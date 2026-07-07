# Quality Checklist — CLI Engineer

## Design Quality
- [ ] Command structure is intuitive
- [ ] Flags are consistent with conventions
- [ ] Sensible defaults provided
- [ ] Help text is comprehensive
- [ ] --help and --version implemented

## Implementation Quality
- [ ] Argument parsing with validation
- [ ] Error messages are informative
- [ ] Exit codes are correct
- [ ] Stdin/stdout/stderr properly handled
- [ ] --json flag for machine output
- [ ] Color output (with NO_COLOR support)

## Shell Integration
- [ ] Shell completions generated (bash, zsh, fish)
- [ ] Environment variable configuration
- [ ] Piping works correctly
- [ ] Configuration file support (if applicable)

## Distribution
- [ ] Cross-platform builds
- [ ] Standalone binary distribution
- [ ] Installation documentation
- [ ] Versioning and changelog