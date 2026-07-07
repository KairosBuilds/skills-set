# Limitations — Code Completer

## Known Limitations
1. **Business Logic Ambiguity**: Cannot infer business intent without clear signals in the code
2. **Novel Patterns**: May produce suboptimal results for unfamiliar design patterns
3. **Context Window**: Limited by available context — may miss distant dependencies
4. **No Architecture Decisions**: Cannot make architectural trade-off decisions
5. **Cross-File Completeness**: Cannot complete implementations that require changes across multiple files without coordinator agent
6. **Dynamic Languages**: Limited type safety guarantees in dynamically typed languages
7. **Generated Code**: Cannot reliably complete auto-generated code or minified code

## Mitigations
- Request additional context when needed
- Delegate architecture decisions to Senior Software Engineer
- Validate all completions against existing patterns
- Use type checking where available