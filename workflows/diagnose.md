# Diagnose Workflow: Root Cause Analysis & System Remediation

**Mission:** [DESCRIBE THE PERSISTENT ISSUE OR SYSTEM FAILURE]

---

## Context

This workflow is for persistent issues where simpler attempts have failed. We need to identify root causes, not just treat symptoms.

---

## Execution Model

This workflow follows a systematic diagnostic approach. Each phase builds on the previous. Announce phase transitions clearly.

---

## Phase 1: Symptom Documentation

**Objective:** Clearly document what's broken, not what we think might be wrong.

**Actions:**
1. **Reproduce the Issue**
   - Can you reproduce it consistently?
   - Under what conditions does it occur?
   - What's the minimal reproduction case?

2. **Gather Evidence**
   - Exact error messages or logs
   - Stack traces
   - Network requests/responses (if applicable)
   - Database state (if applicable)
   - System state at time of failure
   - User-visible impact

3. **Document Symptoms**
   - What happens vs. what should happen?
   - When does it occur? (Always? Sometimes? Specific conditions?)
   - What error messages or logs appear?
   - What's the user-visible impact?

**Deliverable:** Symptom documentation with:
- Exact reproduction steps
- Error logs and stack traces
- System state at failure
- User impact description

**Status:**
- `✅` - Symptoms clearly documented with evidence
- `🚧` - Cannot reproduce (escalate with details)

---

## Phase 2: Hypothesis Generation

**Objective:** Generate multiple hypotheses about potential root causes.

**Actions:**
1. **Analyze Symptoms**
   - What could cause these symptoms?
   - Where in the system could this originate?
   - What assumptions might be wrong?
   - What dependencies could be failing?

2. **Generate Hypotheses**
   - Create multiple potential explanations
   - Consider different layers (frontend, backend, database, infrastructure)
   - Think about timing, state, and dependencies

3. **Prioritize Hypotheses**
   - Most likely first
   - Easiest to verify first
   - Most impactful if true

**Deliverable:** Prioritized hypothesis list with:
- Each hypothesis clearly stated
- Reasoning for each hypothesis
- Priority order with justification

**Status:**
- `✅` - Multiple hypotheses generated and prioritized
- `🚧` - No clear hypotheses (escalate with symptom details)

---

## Phase 3: Hypothesis Testing

**Objective:** Systematically test each hypothesis to identify the root cause.

**Actions:**
1. **Test Each Hypothesis** (in priority order)
   - Design a test to verify or falsify it
   - Execute the test
   - Document results clearly
   - If falsified: move to next hypothesis
   - If verified: proceed to Phase 4

2. **Iterate if Needed**
   - If all hypotheses falsified: generate new hypotheses based on test results
   - Return to Phase 2 with new information
   - Or escalate if truly stuck

**Deliverable:** Root cause identification with:
- Test results for each hypothesis
- Root cause clearly identified
- Evidence supporting the root cause

**Status:**
- `✅` - Root cause identified with evidence
- `⚠️` - Partial understanding, need more investigation
- `🚧` - Cannot identify root cause (escalate with test results)

---

## Phase 4: Remediation

**Objective:** Fix the root cause, not just symptoms.

**Actions:**
1. **Design the Fix**
   - Addresses root cause, not symptoms
   - Doesn't break other functionality
   - Is the simplest solution that works
   - Considers edge cases
   - Includes prevention measures

2. **Implement the Fix**
   - Make the change
   - Test the fix
   - Verify symptoms are resolved
   - Check for regressions

3. **Fix Related Issues**
   - If root cause affected multiple areas, fix all of them
   - Don't just fix the immediate symptom
   - Ensure system consistency

**Deliverable:** Root cause fixed with:
- Fix implementation (with file:line references)
- Verification that symptoms are resolved
- Regression testing results

**Status:**
- `✅` - Fix implemented and verified
- `⚠️` - Fix implemented but issues remain
- `🚧` - Cannot fix (escalate with details)

---

## Phase 5: Prevention & Documentation

**Objective:** Prevent recurrence and document learnings.

**Actions:**
1. **Add Safeguards**
   - Tests to catch this issue
   - Monitoring/alerting if applicable
   - Validation or checks to prevent recurrence
   - Architectural improvements if needed

2. **Update Documentation**
   - What was the root cause?
   - How was it fixed?
   - What should we watch for?
   - Any architectural improvements needed?

3. **Check for Similar Issues**
   - Are there other places with the same pattern?
   - Should we fix those proactively?

**Deliverable:** Prevention measures with:
- Safeguards added (tests, monitoring, validation)
- Documentation updated
- Similar issues addressed (if any)

**Status:**
- `✅` - Prevention measures added, documentation updated
- `⚠️` - Partial prevention (document why)

---

## Final Report Format

```
**Mission:** [THE PERSISTENT ISSUE]

**Phase 1: Symptom Documentation**
- Status: ✅/🚧
- Symptoms: [What's broken]
- Evidence: [Logs, errors, system state]

**Phase 2: Hypothesis Generation**
- Status: ✅/🚧
- Hypotheses: [List, prioritized with reasoning]

**Phase 3: Hypothesis Testing**
- Status: ✅/⚠️/🚧
- Root Cause: [What actually caused it]
- Evidence: [Supporting evidence]

**Phase 4: Remediation**
- Status: ✅/⚠️/🚧
- Fix: [What was changed, with file:line references]
- Verification: [Evidence it's fixed]

**Phase 5: Prevention & Documentation**
- Status: ✅/⚠️
- Prevention: [What was added]
- Documentation: [What was updated]

**Final Verdict:**
- Root cause identified and fixed. Prevention measures in place. Mission accomplished.
```

---

**Begin Phase 1: Symptom Documentation**

