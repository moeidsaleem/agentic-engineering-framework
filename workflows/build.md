---
layout: default
title: Build Workflow
description: Feature development & system enhancement workflow
---

# Build Workflow: Feature Development & System Enhancement

**Mission:** [YOUR HIGH-LEVEL GOAL HERE]

---

## Execution Model

This workflow guides you through systematic feature development or system enhancement. Each phase must complete before proceeding. Announce phase transitions clearly.

---

## Phase 1: Discovery

**Objective:** Understand the current system state without making changes.

**Actions:**
1. **Documentation Review**
   - Search workspace: `notes/`, `docs/`, README files
   - Check user home: `~/Documents/Documentation/`, `~/Documents/Notes/`
   - Review project `.md` files, ADRs, wikis
   - Note: Documentation may be outdated—verify against code

2. **System Architecture Mapping**
   - Data flow: Request lifecycle, transformation points
   - Dependencies: Integration points, service dependencies
   - Configuration: Environment variables, service configs
   - Existing implementations: Search for similar features to leverage/expand

3. **Code Pattern Analysis**
   - Study existing code that solves similar problems
   - Identify architectural patterns
   - Map component relationships
   - Trace dependencies for any code you plan to extend

**Deliverable:** Discovery report with:
- Current system state summary
- Relevant existing implementations (with file paths)
- Architecture and data flow diagram (textual)
- Dependencies and integration points
- Potential risks or blockers

**Status:**
- `✅` - Discovery complete, no blockers identified
- `⚠️` - Issues found that need addressing
- `🚧` - Blocked by missing information or ambiguous requirements

---

## Phase 2: Strategy

**Objective:** Design the solution approach before implementation.

**Actions:**
1. **Solution Design**
   - How will this integrate with existing code?
   - Which components need modification?
   - What new components (if any) are needed?
   - How will this be tested?

2. **Risk Assessment**
   - What could break?
   - What edge cases exist?
   - What performance implications?
   - What security considerations?

3. **Blocker Check**
   - Ambiguous requirements?
   - Multiple valid architectural choices?
   - Security/risk concerns?
   - Missing critical information?

**Deliverable:** Strategy document with:
- Approach and rationale
- Components to modify/create (with file paths)
- Testing strategy
- Risk mitigation plan

**If blocked:** Escalate immediately with specific questions. Do not proceed until unblocked.

**If unblocked:** Proceed to Phase 3 immediately.

---

## Phase 3: Execution

**Objective:** Implement the solution autonomously with continuous verification.

**Actions:**
1. **Implementation**
   - Execute the strategy
   - Make changes incrementally
   - Test after each significant change

2. **Continuous Verification**
   - Run relevant tests after each change
   - Fix issues discovered immediately
   - Verify changes work as intended
   - Check for regressions

3. **Complete Task Chains**
   - If Task A reveals Issue B: understand both, fix both
   - Don't stop at first problem
   - Chain related fixes until system works
   - Fix entire problem sets, not individual symptoms

**Deliverable:** Working implementation with:
- All code changes (with file:line references)
- Tests passing
- No lint errors
- Integration verified
- Documentation updated (if needed)

**Status:**
- `✅` - Implementation complete and verified
- `⚠️` - Recoverable issues encountered and fixed
- `🚧` - Blocked during execution (escalate with specific questions)

---

## Phase 4: Validation

**Objective:** Prove the work is correct and complete.

**Actions:**
1. **End-to-End Verification**
   - Does it actually work? (Not just build, but function correctly)
   - Are integration points tested?
   - Are edge cases considered?
   - Is anything exposed that shouldn't be?
   - Will this perform okay?

2. **Completeness Check**
   - All related issues resolved?
   - Documentation updated?
   - Temp files cleaned up?
   - No debug code or console.logs?
   - Workspace clean?

3. **Final Verification**
   - Tests pass
   - Lint clean
   - Build successful
   - System state consistent

**Deliverable:** Validation report with:
- Verification evidence (test output, build status)
- Summary of changes (with file:line references)
- System state confirmation

---

## Final Report Format

```
**Mission:** [YOUR HIGH-LEVEL GOAL]

**Phase 1: Discovery**
- Status: ✅/⚠️/🚧
- Findings: [Summary with file paths]

**Phase 2: Strategy**
- Status: ✅/⚠️/🚧
- Approach: [Summary]
- Components: [List with paths]

**Phase 3: Execution**
- Status: ✅/⚠️/🚧
- Changes: [Summary with file:line references]

**Phase 4: Validation**
- Verification Evidence:
  - [Test output, build status, etc.]
- Final Verdict:
  - Build complete. System state verified and consistent. Mission accomplished.
```

---

**Begin Phase 1: Discovery**
