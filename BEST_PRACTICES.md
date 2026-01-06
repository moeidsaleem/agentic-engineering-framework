# Best Practices Library

**Author:** Moeid Saleem Khan  
**Version:** 2.0

Curated learnings and patterns from real-world usage of the framework.

---

## Investigation Best Practices

### 1. Start with Code, Not Docs
- Read actual code first to understand reality
- Use documentation for intent and context
- Always verify docs against code

### 2. Map Dependencies First
- Understand what depends on what
- Trace imports and references
- Identify circular dependencies early

### 3. Find Similar Implementations
- Search for existing solutions before creating new
- Leverage and extend existing code
- Maintain consistency with existing patterns

### 4. Verify Before Changing
- Understand current behavior
- Test current state
- Document what you're changing and why

---

## Execution Best Practices

### 1. Test Incrementally
- Test after each significant change
- Don't wait until the end
- Catch issues early

### 2. Fix Complete Chains
- If you find Issue A, look for Issues B, C, D
- Fix the entire problem set
- Don't stop at symptoms

### 3. Update Documentation
- Keep docs current with code
- Update immediately after changes
- Don't create duplicates

### 4. Clean as You Go
- Remove temp files immediately
- Delete debug code
- Keep workspace clean

---

## Communication Best Practices

### 1. Be Specific
- Use file:line references
- Provide evidence
- State facts, not opinions

### 2. Show, Don't Tell
- Provide code examples
- Include test output
- Show verification results

### 3. Escalate Clearly
- State what's blocking you
- Explain what you've tried
- Ask specific questions

### 4. Report Progress Meaningfully
- Only report when there's substance
- Use status markers
- Provide actionable information

---

## Security Best Practices

### 1. Never Hardcode Secrets
- Use environment variables
- Check .env files
- Use credential management tools

### 2. Validate Inputs
- Always validate user input
- Sanitize data
- Use parameterized queries

### 3. Follow Least Privilege
- Use minimal required permissions
- Don't expose unnecessary data
- Secure API endpoints

### 4. Review Security Implications
- Consider security in every change
- Review authentication/authorization
- Check for injection vulnerabilities

---

## Performance Best Practices

### 1. Measure Before Optimizing
- Profile first
- Identify actual bottlenecks
- Don't optimize prematurely

### 2. Watch for Common Issues
- N+1 queries
- Memory leaks
- Unnecessary re-renders
- Inefficient algorithms

### 3. Test Performance
- Benchmark before and after
- Test with realistic data volumes
- Monitor in production

### 4. Optimize Incrementally
- Make one change at a time
- Measure impact
- Verify improvements

---

## Code Quality Best Practices

### 1. Follow Existing Patterns
- Match project conventions
- Use established patterns
- Maintain consistency

### 2. Write Testable Code
- Keep functions pure when possible
- Minimize side effects
- Make dependencies explicit

### 3. Keep It Simple
- Prefer simple solutions
- Avoid over-engineering
- Don't add unnecessary abstraction

### 4. Document Decisions
- Explain WHY, not just WHAT
- Document trade-offs
- Note assumptions

---

## Error Handling Best Practices

### 1. Handle Errors Gracefully
- Provide meaningful error messages
- Log errors appropriately
- Don't expose internals

### 2. Fail Fast
- Validate early
- Check prerequisites
- Don't proceed with invalid state

### 3. Provide Recovery Paths
- Suggest solutions
- Provide rollback options
- Enable graceful degradation

### 4. Test Error Cases
- Test failure scenarios
- Verify error messages
- Check recovery procedures

---

## Documentation Best Practices

### 1. Keep It Current
- Update immediately after changes
- Remove outdated information
- Verify accuracy

### 2. Be Specific
- Include examples
- Provide code samples
- Show actual usage

### 3. Document Why
- Explain decisions
- Note trade-offs
- Record assumptions

### 4. Organize Logically
- Group related information
- Use clear headings
- Provide navigation

---

## Testing Best Practices

### 1. Test Behavior, Not Implementation
- Test what it does, not how
- Focus on outcomes
- Avoid brittle tests

### 2. Test Integration Points
- Test how components interact
- Verify data flow
- Check error propagation

### 3. Test Edge Cases
- Boundary conditions
- Error scenarios
- Unusual inputs

### 4. Keep Tests Maintainable
- Clear test names
- Isolated tests
- Fast execution

---

## Git Best Practices

### 1. Use Descriptive Commits
- Explain what changed
- Explain why it changed
- Reference issues if applicable

### 2. Follow Branch Workflow
- Feature branches from `develop`
- PRs to `develop`
- Never PR directly to `main` or `staging`

### 3. Keep History Clean
- Logical commit grouping
- Meaningful commit messages
- Avoid unnecessary merges

### 4. Review Before Merging
- Self-review your changes
- Check for issues
- Verify tests pass

---

## Framework Usage Best Practices

### 1. Choose the Right Workflow
- `build.md` for features
- `diagnose.md` for bugs
- `migrate.md` for migrations
- `evolve.md` for learning

### 2. Use Modifiers Appropriately
- `terse.md` for speed
- `professional.md` for formal tone
- Stack as needed

### 3. Customize for Your Needs
- Adapt workflows to your domain
- Extend manifest with project rules
- Maintain core principles

### 4. Learn and Improve
- Use `evolve.md` regularly
- Capture patterns that work
- Improve the framework

---

## Common Patterns

### Pattern: Leverage Before Create
- Always search for existing solutions
- Extend existing code when possible
- Maintain consistency

### Pattern: Verify Before Trust
- Trust code over docs
- Verify assumptions
- Test actual behavior

### Pattern: Fix Chains, Not Symptoms
- Find root causes
- Fix entire problem sets
- Ensure system consistency

### Pattern: Test Continuously
- Test after each change
- Verify integration points
- Don't wait until end

---

## Anti-Patterns to Avoid

### ❌ Assuming Documentation is Current
- Always verify against code
- Don't trust docs blindly
- Update docs after changes

### ❌ Stopping at First Issue
- Fix entire problem chains
- Don't stop at symptoms
- Ensure completeness

### ❌ Testing Only at the End
- Test incrementally
- Verify continuously
- Catch issues early

### ❌ Creating Instead of Leveraging
- Search for existing solutions
- Extend existing code
- Maintain consistency

### ❌ Skipping Investigation
- Always investigate first
- Understand before changing
- Map dependencies

---

## Success Metrics

Track these to measure framework effectiveness:

1. **Completion Rate** - Tasks completed successfully
2. **Issue Discovery** - Problems found and fixed
3. **Documentation Currency** - Docs updated with changes
4. **Code Quality** - Tests pass, lint clean
5. **System Consistency** - No regressions introduced
6. **Time to Resolution** - How quickly issues are resolved
7. **Framework Evolution** - Improvements captured via evolve workflow

---

**Remember: Best practices evolve. Use `workflows/evolve.md` to capture new learnings and improve this library.**

