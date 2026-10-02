# Copilot Agent Instructions – Java 17

## Objective
Analyze the provided prompt and existing codebase to implement the requested change with minimal, precise modifications.

The agent must:
- Identify exactly what needs to change
- Modify only the impacted components
- Produce clean, optimized, production-ready Java 17 code

---

## Mandatory Workflow

### 1. Prompt Analysis
Before writing any code, the agent MUST:
- Fully understand the requirement
- Identify:
    - What must change
    - What must remain unchanged
    - Impacted classes, methods, and components

DO NOT start coding before completing this analysis.

---

### 2. Impact Analysis
- Determine the exact scope of the change
- Modify ONLY:
    - Relevant methods
    - Related classes if strictly required

AVOID:
- Wide refactoring
- Changes to unrelated modules

---

### 3. Targeted Code Changes
- Apply changes only to impacted components
- Preserve:
    - Existing logic unless incorrect
    - Backward compatibility

Ensure no regressions are introduced.

---

## Java Standards

### 4. Java Version
- Use Java 17 ONLY

DO NOT use:
- `var` keyword
- Deprecated APIs

---

### 5. Java 17 Best Practices
Use modern language features only when they improve clarity or correctness:
- Records (DTOs)
- Sealed classes (when applicable)
- Switch expressions
- Pattern matching for `instanceof`
- Optional for nullable values
- Stream API (readable usage only)

Do not over-engineer.

---

## Code Quality Requirements

### 6. Optimization
- Favor optimal time and space complexity
- Avoid redundant computation
- Avoid unnecessary object creation
- Prefer immutability

---

### 7. Tech Stack Alignment
- Prefer standard Java libraries
- Use clean, modern APIs

Avoid legacy patterns and outdated frameworks unless explicitly required.

---

### 8. Design Principles
Apply only if they clearly improve the solution:
- SOLID
- DRY
- KISS

Do not introduce abstractions without justification.

---

### 9. Design Patterns
Use only when they add clear value:
- Strategy
- Factory
- Builder
- Singleton (only if explicitly justified)

Do not introduce patterns by default.

---

### 10. Loose Coupling
- Minimize dependencies
- Prefer interfaces over implementations
- Use dependency injection where appropriate

Avoid tight coupling and hard dependencies.

---

### 11. Clean Code
- Use meaningful names
- Keep methods small and focused
- Avoid deep nesting
- Maintain consistent formatting

---

### 12. Error Handling
- Handle errors explicitly
- Use specific exceptions

Avoid:
- Silent failures
- Catching generic `Exception`

---

### 13. Null Safety
- Prevent `NullPointerException`
- Validate external inputs
- Use `Optional` where appropriate

---

### 14. Logging
- Add logging only if it provides meaningful diagnostics
- Avoid excessive or noisy logs

---

## Output Rules

### 15. Response Constraints
The agent MUST return:
- Only modified or newly added code
- Clean, formatted, compilable Java code
- No explanations or commentary

---

### 16. Final Validation
Before responding, verify:
- Code compiles
- No unused imports or variables
- No performance regressions
- All rules in this document are satisfied

---

## Enforcement Rule
If rules conflict:
- Prefer simplicity over complexity
- Prefer minimal change over full refactor