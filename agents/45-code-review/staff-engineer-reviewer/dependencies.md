# Examples

## Example 1: Over-Engineering Detection
`	ypescript
// ❌ Over-engineered with unnecessary abstraction
interface IUserRepositoryFactoryProviderStrategy { ... }

// ✅ Simple and sufficient
class UserRepository { ... }
`

## Example 2: Missing Abstraction
`	ypescript
// ❌ Business logic scattered in controller
function handleOrder(req, res) {
  // 50 lines of order processing logic
}

// ✅ Separated concerns
// Controller delegates to service layer
`

## Example 3: Tight Coupling
`	ypescript
// ❌ Service directly instantiates dependencies
class OrderService {
  private db = new MySQLDatabase();
}

// ✅ Dependency injection
class OrderService {
  constructor(private db: Database) {}
}
`
"@ | Set-Content -Path "C:\Users\black\Downloads\IRIS-AI-1.3.0\IRIS-AI-1.3.0\.opencode\agents\review\staff-engineer-reviewer\examples.md" -Encoding UTF8

@"
# Dependencies

## Internal Dependencies
- code-quality/staff-engineer-review (skill)
- architecture/architecture-designer (skill)
- code-quality/code-reviewer (skill)

## External Tools
- SonarQube (architecture analysis)
- Structure101 (dependency analysis)
- NDepend (.NET architecture)
- JQAssistant (architecture validation)

## Runtime
- Node.js >= 18
- Python >= 3.10
- Java >= 17 (for Java analysis)
