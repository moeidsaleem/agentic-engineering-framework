# Framework Structure

```
Cursor-prompt-guidelines/
├── README.md                    # Main overview and usage guide
├── manifest.md                  # The Engineering Agent Manifest (core rules)
├── LICENSE                      # MIT License
├── STRUCTURE.md                 # This file
├── QUICK_REFERENCE.md           # Cheat sheet for common scenarios
├── TROUBLESHOOTING.md           # Common issues and solutions
├── BEST_PRACTICES.md            # Curated learnings and patterns
├── SECURITY_CHECKLIST.md        # Security review checklist
├── workflows/
│   ├── build.md                # Feature development & system enhancement
│   ├── diagnose.md             # Root cause analysis & remediation
│   ├── migrate.md              # Data migration & system transformation
│   └── evolve.md               # Framework improvement & learning capture
├── modifiers/
│   ├── terse.md                # Ultra-concise communication mode
│   └── professional.md         # Eliminates sycophantic language
└── examples/
    └── example-build.md        # Real-world build workflow example
```

## Key Differences from Original Framework

### Naming Conventions
- **Manifest** (instead of "Doctrine") - More modern, engineering-focused terminology
- **Workflows** (instead of "Playbooks") - Emphasizes systematic execution
- **Modifiers** (instead of "Directives") - Clearer purpose as behavior adjustments

### Improved Structure
- **Clearer phase naming** - Discovery, Strategy, Execution, Validation (instead of Reconnaissance, Planning, etc.)
- **Better organization** - More logical flow and separation of concerns
- **Enhanced execution model** - More systematic approach to each workflow

### Enhanced Features
- **System-wide thinking** - Emphasized throughout
- **Better verification** - More comprehensive validation phases
- **Improved learning loop** - Evolve workflow captures and applies learnings
- **Quick reference guide** - Fast lookup for common scenarios
- **Troubleshooting guide** - Solutions for common issues
- **Best practices library** - Curated learnings from real usage
- **Security checklist** - Comprehensive security review
- **Real-world examples** - Practical usage demonstrations
- **Migration workflow** - Specialized workflow for data migrations

### Branch Workflow Fix
- **Corrected git workflow**: `develop` → `staging` → `main`
- PRs from feature branches to `develop`
- Never PR directly to `main` or `staging`

## Author

**Moeid Saleem Khan**

---

**Version:** 2.0  
**Last Updated:** 2026-01-06

