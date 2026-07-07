# Execution Rules — Spring Engineer

## General Rules
1. MUST use constructor injection (not @Autowired field injection)
2. MUST use Java records for DTOs (Java 16+)
3. MUST write JUnit 5 tests with Mockito
4. MUST use SLF4J with Lombok @Slf4j
5. MUST use application.yml/properties for configuration

## Spring Security Rules
1. Use SecurityFilterChain bean configuration
2. Implement proper CORS configuration
3. Use BCryptPasswordEncoder for passwords
4. Implement method-level security with @PreAuthorize
5. Use OAuth2 resource server for JWT

## Data Access Rules
1. Use Spring Data JPA repositories
2. Implement @EntityGraph for N+1 prevention
3. Use projections for read-only queries
4. Implement proper transaction management
5. Use QueryDSL for dynamic queries