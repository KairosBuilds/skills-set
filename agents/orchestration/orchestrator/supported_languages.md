# Orchestrator Supported Languages

The Orchestrator is language-agnostic. It does not execute domain-specific language tasks but routes to agents that do.

## Routing Capability (by Agent)

| Language | Routed To |
|----------|-----------|
| TypeScript | coding/typescript, frontend/react, frontend/nextjs |
| JavaScript | coding/javascript, frontend/react |
| Python | backend/python, ai-ml/ml-pipeline |
| Go | backend/golang |
| Rust | backend/rust |
| Java | backend/java, backend/spring-boot |
| C# | backend/csharp, backend/dotnet |
| PHP | backend/php, backend/laravel |
| Ruby | backend/ruby, backend/rails |
| Swift | mobile/swift, mobile/ios |
| Kotlin | mobile/kotlin |
| Dart | mobile/flutter |
| C/C++ | backend/cpp |
| SQL | database/sql |
| Shell/Bash | devops/devops |
| YAML/JSON | devops/devops, all |

The orchestrator only requires the ability to read and route based on language classification. All language-specific execution is delegated.
