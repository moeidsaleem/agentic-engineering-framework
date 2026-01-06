# Quick Reference Guide

**Author:** Moeid Saleem Khan  
**Version:** 2.0

A cheat sheet for common scenarios and quick lookups.

---

## Workflow Selection Matrix

| Scenario | Workflow | Modifiers |
|----------|----------|-----------|
| Building new feature | `workflows/build.md` | `terse.md` for speed |
| Fixing a bug | `workflows/diagnose.md` | - |
| Refactoring code | `workflows/build.md` | - |
| Persistent issue | `workflows/diagnose.md` | - |
| End of session | `workflows/evolve.md` | - |
| Quick fix | `workflows/build.md` | `terse.md` |
| Complex debugging | `workflows/diagnose.md` | - |
| Learning capture | `workflows/evolve.md` | - |

---

## Status Indicators

- `✅` - Objective completed successfully
- `⚠️` - Issue encountered and resolved autonomously
- `🚧` - Blocked, requires human input
- `🔍` - Investigation in progress

---

## Common Commands

### Installation
```bash
# Copy manifest.md content to Cursor rules
# Global: Settings → Rules → Add Rule
# Project: .cursorrules or .cursor/rules/manifest.md
```

### Quick Workflow Usage
1. Open workflow file
2. Replace `[YOUR HIGH-LEVEL GOAL HERE]` with your goal
3. (Optional) Append modifier content
4. Paste into chat

---

## Investigation Checklist

Before making changes, verify:
- [ ] Documentation reviewed (may be outdated)
- [ ] Code patterns studied
- [ ] Dependencies mapped
- [ ] Similar implementations found
- [ ] System architecture understood
- [ ] Risks identified
- [ ] Blockers checked

---

## Execution Checklist

Before marking complete:
- [ ] Actually works (not just compiles)
- [ ] Integration points tested
- [ ] Edge cases considered
- [ ] Security reviewed
- [ ] Performance acceptable
- [ ] Documentation updated
- [ ] Workspace clean
- [ ] Tests pass
- [ ] Lint clean

---

## Branch Workflow

```
feature/branch-name
    ↓ (PR)
develop
    ↓ (merge)
staging
    ↓ (merge)
main
```

**Never PR directly to `main` or `staging`**

---

## File Operation Rules

**Use file tools for:**
- Reading files
- Editing files
- Creating files
- Searching content

**Use bash for:**
- Git operations
- Package managers
- Process management
- System commands

---

## Credential Locations

1. `AGENTS.md` - Service documentation
2. `.env` files - API keys, tokens
3. `~/.config`, `~/.ssh` - Global config
4. CLI tools - AWS CLI, `gh`, etc.
5. `scripts/` - Existing wrappers

---

## Search Safety

- Use `head_limit` (20-50)
- Specify path when possible
- Start narrow, expand gradually
- Don't repeat failed searches
- Verify directory structure first

---

## Communication Standards

**Do:**
- Be direct and technical
- Use file:line references
- Provide evidence
- State facts, not opinions

**Don't:**
- Use emojis in commits
- Add conversational filler
- Validate non-factual statements
- Provide status without substance

---

## Escalation Triggers

Escalate when:
- Requirements ambiguous
- Multiple valid approaches
- Security/risk concerns
- Missing critical info
- User explicitly requested review

---

## Quick Tips

1. **Trust code over docs** - Always verify
2. **Fix entire chains** - Don't stop at symptoms
3. **Build for reuse** - Check scripts/ first
4. **Test as you build** - Don't wait until end
5. **Update docs** - Keep them current
6. **Clean workspace** - Remove temp files
7. **Use absolute paths** - Eliminate confusion
8. **Stack modifiers** - Combine as needed

---

**For detailed information, see the full documentation in README.md and manifest.md**

