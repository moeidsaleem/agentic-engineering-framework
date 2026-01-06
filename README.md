# The Agentic Engineering Framework

**Author:** Moeid Saleem Khan  
**Version:** 2.0  
**Last Updated:** 2026-01-06

A systematic, evidence-driven framework designed to transform AI agents into autonomous engineering partners capable of independent problem-solving, system-wide thinking, and continuous self-improvement.

**Core Philosophy:** *Precision through investigation. Autonomy through discipline. Excellence through verification.*

---

## What Makes This Framework Different

This framework goes beyond simple prompting rules. It's a complete operational system that:

- **Emphasizes system thinking** - Every action considers end-to-end impact
- **Prioritizes verification** - Trust is earned through evidence, not assumptions
- **Enables true autonomy** - Agents make decisions within clear guardrails
- **Learns continuously** - Built-in feedback loops improve the framework itself
- **Scales with complexity** - Adapts from simple tasks to architectural changes

---

## Framework Architecture

The framework consists of three integrated layers:

### 1. The Engineering Manifest (`manifest.md`)

The foundational constitution that defines agent behavior, decision-making protocols, and quality standards. This is the single source of truth for all agent operations.

**Installation:**
- **Global (Recommended):** Install as a global rule in your AI environment for workspace-wide consistency
- **Project-Specific:** Place in `.cursor/rules/` or project root `AGENT.md` for project-specific overrides

> **Important:** Treat the Manifest as infrastructure-as-code. When updating, replace the entire file to prevent configuration drift.

**Links:**
- [View manifest.md](manifest.md) | [GitHub](https://github.com/moeidsaleem/agentic-engineering-framework/blob/main/manifest.md) | [Raw](https://raw.githubusercontent.com/moeidsaleem/agentic-engineering-framework/main/manifest.md)

### 2. The Workflow Templates (`workflows/`)

Structured execution templates that guide agents through specific task types. Each workflow enforces a rigorous, repeatable process.

**Status Indicators:**
- `✅` - Objective completed successfully
- `⚠️` - Issue encountered and resolved autonomously
- `🚧` - Blocked, requires human input
- `🔍` - Investigation in progress

| Workflow | Purpose | When to Use | Links |
|----------|---------|-------------|-------|
| **build.md** | Feature development & system enhancement | Creating new features, refactoring, planned improvements | [View](workflows/build.md) \| [GitHub](https://github.com/moeidsaleem/agentic-engineering-framework/blob/main/workflows/build.md) \| [Raw](https://raw.githubusercontent.com/moeidsaleem/agentic-engineering-framework/main/workflows/build.md) |
| **diagnose.md** | Deep debugging & root cause analysis | Persistent bugs, system failures, complex issues | [View](workflows/diagnose.md) \| [GitHub](https://github.com/moeidsaleem/agentic-engineering-framework/blob/main/workflows/diagnose.md) \| [Raw](https://raw.githubusercontent.com/moeidsaleem/agentic-engineering-framework/main/workflows/diagnose.md) |
| **migrate.md** | Data migration & system transformation | Database migrations, schema changes, data transformations | [View](workflows/migrate.md) \| [GitHub](https://github.com/moeidsaleem/agentic-engineering-framework/blob/main/workflows/migrate.md) \| [Raw](https://raw.githubusercontent.com/moeidsaleem/agentic-engineering-framework/main/workflows/migrate.md) |
| **evolve.md** | Framework improvement & learning capture | End of session to improve the framework itself | [View](workflows/evolve.md) \| [GitHub](https://github.com/moeidsaleem/agentic-engineering-framework/blob/main/workflows/evolve.md) \| [Raw](https://raw.githubusercontent.com/moeidsaleem/agentic-engineering-framework/main/workflows/evolve.md) |

### 3. The Behavior Modifiers (`modifiers/`)

Optional, stackable behavior adjustments that can be appended to workflows for specific communication styles or operational modes.

| Modifier | Effect | Links |
|----------|--------|-------|
| **terse.md** | Ultra-concise, information-dense communication | [View](modifiers/terse.md) \| [GitHub](https://github.com/moeidsaleem/agentic-engineering-framework/blob/main/modifiers/terse.md) \| [Raw](https://raw.githubusercontent.com/moeidsaleem/agentic-engineering-framework/main/modifiers/terse.md) |
| **professional.md** | Eliminates sycophantic language and filler | [View](modifiers/professional.md) \| [GitHub](https://github.com/moeidsaleem/agentic-engineering-framework/blob/main/modifiers/professional.md) \| [Raw](https://raw.githubusercontent.com/moeidsaleem/agentic-engineering-framework/main/modifiers/professional.md) |

---

## Quick Start: Your First Session

### Step 1: Install the Manifest

Copy the contents of `manifest.md` into your Cursor rules (global or project-specific).

### Step 2: Choose Your Workflow

Select the appropriate workflow template:
- **Building something new?** → Use `workflows/build.md`
- **Debugging a persistent issue?** → Use `workflows/diagnose.md`
- **Wrapping up a session?** → Use `workflows/evolve.md`

### Step 3: Customize and Execute

1. Open the workflow file
2. Replace the mission placeholder with your specific goal
3. (Optional) Append a modifier if you need specific behavior
4. Paste the entire text into your chat
5. Observe the structured execution

### Step 4: Review and Learn

After completion, use `workflows/evolve.md` to capture learnings and improve the framework.

---

## The Execution Model

Every workflow follows a structured execution model:

1. **Discovery Phase** - Non-destructive investigation of current state
2. **Strategy Phase** - Planning with risk assessment and dependency mapping
3. **Execution Phase** - Autonomous implementation with continuous verification
4. **Validation Phase** - Comprehensive testing and system consistency checks
5. **Documentation Phase** - Update docs, clean workspace, report findings

Each phase must complete before proceeding. Blockers are escalated immediately with specific questions.

---

## Core Principles

1. **Evidence Over Assumption** - Every decision backed by investigation
2. **System-Wide Ownership** - Fix entire problem chains, not just symptoms
3. **Autonomous Execution** - Act within guardrails, escalate only when truly blocked
4. **Continuous Verification** - Test as you build, verify before completion
5. **Self-Improvement** - Framework evolves based on real-world usage

---

## Advanced Usage

### Stacking Modifiers

You can combine multiple modifiers for specific scenarios:

```
[workflow content]
---
[modifier 1 content]
---
[modifier 2 content]
```

### Custom Workflows

Create project-specific workflows by adapting the templates. Maintain the core execution model but customize phases for your domain.

### Manifest Customization

The Manifest can be extended with project-specific rules. Add sections that complement (don't contradict) the core principles.

---

## Additional Resources

### Quick Reference
- **[QUICK_REFERENCE.md](QUICK_REFERENCE.md)** - Cheat sheet for common scenarios and quick lookups
- [View on GitHub](https://github.com/moeidsaleem/agentic-engineering-framework/blob/main/QUICK_REFERENCE.md) | [Raw](https://raw.githubusercontent.com/moeidsaleem/agentic-engineering-framework/main/QUICK_REFERENCE.md)

### Examples
- **[examples/example-build.md](examples/example-build.md)** - Real-world example of build workflow in action
- [View on GitHub](https://github.com/moeidsaleem/agentic-engineering-framework/blob/main/examples/example-build.md) | [Raw](https://raw.githubusercontent.com/moeidsaleem/agentic-engineering-framework/main/examples/example-build.md)

### Troubleshooting
- **[TROUBLESHOOTING.md](TROUBLESHOOTING.md)** - Common issues and solutions
- [View on GitHub](https://github.com/moeidsaleem/agentic-engineering-framework/blob/main/TROUBLESHOOTING.md) | [Raw](https://raw.githubusercontent.com/moeidsaleem/agentic-engineering-framework/main/TROUBLESHOOTING.md)

### Best Practices
- **[BEST_PRACTICES.md](BEST_PRACTICES.md)** - Curated learnings and patterns from real-world usage
- [View on GitHub](https://github.com/moeidsaleem/agentic-engineering-framework/blob/main/BEST_PRACTICES.md) | [Raw](https://raw.githubusercontent.com/moeidsaleem/agentic-engineering-framework/main/BEST_PRACTICES.md)

### Security
- **[SECURITY_CHECKLIST.md](SECURITY_CHECKLIST.md)** - Comprehensive security review checklist
- [View on GitHub](https://github.com/moeidsaleem/agentic-engineering-framework/blob/main/SECURITY_CHECKLIST.md) | [Raw](https://raw.githubusercontent.com/moeidsaleem/agentic-engineering-framework/main/SECURITY_CHECKLIST.md)

### Specialized Workflows
- **[workflows/migrate.md](workflows/migrate.md)** - For data migrations and system transformations
- [View on GitHub](https://github.com/moeidsaleem/agentic-engineering-framework/blob/main/workflows/migrate.md) | [Raw](https://raw.githubusercontent.com/moeidsaleem/agentic-engineering-framework/main/workflows/migrate.md)

---

## Contributing & Evolution

This framework is designed to evolve. Use `workflows/evolve.md` regularly to:
- Capture patterns that work
- Identify framework gaps
- Propose improvements
- Update the Manifest based on real-world learnings

---

## Credits

**Framework Author:** Moeid Saleem Khan

**Inspired by:** The need for systematic, evidence-driven AI agent behavior in complex engineering environments.

---

## License

This framework is provided as-is for use in AI-assisted development workflows. Customize freely for your needs.

---

**Welcome to systematic, autonomous, evidence-driven AI engineering.**
