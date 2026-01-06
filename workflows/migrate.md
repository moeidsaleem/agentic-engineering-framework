# Migrate Workflow: Data Migration & System Transformation

**Mission:** [DESCRIBE THE MIGRATION OR TRANSFORMATION TASK]

---

## Context

This workflow is for data migrations, schema changes, system transformations, or any operation that moves or transforms data across systems. These operations require extra care due to data loss risks.

---

## Execution Model

This workflow follows a careful, reversible approach to migrations. Each phase must complete before proceeding. Announce phase transitions clearly.

---

## Phase 1: Discovery

**Objective:** Understand the current state, target state, and migration requirements.

**Actions:**
1. **Source System Analysis**
   - Current data structure and schema
   - Data volume and growth patterns
   - Dependencies and relationships
   - Data quality issues
   - Access patterns and usage

2. **Target System Analysis**
   - Target schema and structure
   - Migration requirements
   - Compatibility considerations
   - Performance requirements
   - Validation rules

3. **Migration Path Mapping**
   - Data transformation requirements
   - Dependency order
   - Rollback strategy
   - Validation checkpoints
   - Risk assessment

**Deliverable:** Migration analysis with:
- Source system state
- Target system requirements
- Migration path and dependencies
- Risk assessment
- Rollback strategy

**Status:**
- `✅` - Discovery complete, migration path clear
- `⚠️` - Risks identified, mitigation needed
- `🚧` - Blocked by missing information or unclear requirements

---

## Phase 2: Strategy

**Objective:** Design a safe, reversible migration plan.

**Actions:**
1. **Migration Design**
   - Step-by-step migration plan
   - Data transformation logic
   - Validation at each step
   - Rollback procedures
   - Performance optimization

2. **Safety Measures**
   - Backup strategy
   - Validation checkpoints
   - Rollback triggers
   - Monitoring and alerting
   - Testing in isolation

3. **Risk Mitigation**
   - Data loss prevention
   - Downtime minimization
   - Performance impact
   - Dependency management
   - Failure recovery

**Deliverable:** Migration strategy with:
- Detailed migration plan
- Safety measures
- Risk mitigation
- Rollback procedures
- Testing strategy

**If blocked:** Escalate immediately. Do not proceed with unclear migration requirements.

**If unblocked:** Proceed to Phase 3.

---

## Phase 3: Preparation

**Objective:** Set up migration infrastructure and test in isolation.

**Actions:**
1. **Backup Creation**
   - Full backup of source data
   - Verify backup integrity
   - Store backup securely
   - Document backup location

2. **Migration Scripts**
   - Create migration scripts
   - Add validation checkpoints
   - Include rollback logic
   - Add logging and monitoring

3. **Test in Isolation**
   - Test on sample data
   - Test on staging environment
   - Verify data integrity
   - Test rollback procedures
   - Performance testing

**Deliverable:** Prepared migration with:
- Backups created and verified
- Migration scripts ready
- Tested in isolation
- Rollback procedures verified

**Status:**
- `✅` - Preparation complete, ready to execute
- `⚠️` - Issues found, need resolution
- `🚧` - Blocked (escalate)

---

## Phase 4: Execution

**Objective:** Execute migration with continuous validation.

**Actions:**
1. **Pre-Migration Validation**
   - Verify source data state
   - Confirm backup integrity
   - Check system readiness
   - Validate migration scripts

2. **Migration Execution**
   - Execute migration in steps
   - Validate at each checkpoint
   - Monitor for issues
   - Log all operations

3. **Post-Migration Validation**
   - Verify data integrity
   - Check data completeness
   - Validate transformations
   - Test system functionality
   - Performance verification

**Deliverable:** Migration executed with:
- Migration steps completed
- Validation results
- Data integrity confirmed
- System functionality verified

**Status:**
- `✅` - Migration complete and verified
- `⚠️` - Issues encountered, need resolution
- `🚧` - Migration failed, rollback needed

---

## Phase 5: Verification & Cleanup

**Objective:** Verify migration success and clean up.

**Actions:**
1. **Comprehensive Verification**
   - Data integrity checks
   - System functionality tests
   - Performance benchmarks
   - User acceptance (if applicable)

2. **Documentation**
   - Document migration process
   - Update system documentation
   - Record any issues encountered
   - Update runbooks

3. **Cleanup**
   - Remove migration scripts (or archive)
   - Clean up temp files
   - Update monitoring
   - Archive backups (keep for rollback period)

**Deliverable:** Migration verified with:
- Verification results
- Documentation updated
- Cleanup complete

---

## Final Report Format

```
**Mission:** [MIGRATION TASK]

**Phase 1: Discovery**
- Status: ✅/⚠️/🚧
- Source: [Summary]
- Target: [Summary]
- Migration Path: [Summary]

**Phase 2: Strategy**
- Status: ✅/⚠️/🚧
- Plan: [Summary]
- Safety: [Measures]

**Phase 3: Preparation**
- Status: ✅/⚠️/🚧
- Backups: [Location and verification]
- Scripts: [Ready and tested]

**Phase 4: Execution**
- Status: ✅/⚠️/🚧
- Steps: [Completed]
- Validation: [Results]

**Phase 5: Verification & Cleanup**
- Status: ✅/⚠️
- Verification: [Results]
- Documentation: [Updated]

**Final Verdict:**
- Migration complete. Data integrity verified. System operational. Mission accomplished.
```

---

## Special Considerations

1. **Always have a rollback plan** - Migrations can fail
2. **Test in isolation first** - Never test on production data directly
3. **Validate continuously** - Check data at each step
4. **Monitor closely** - Watch for performance issues
5. **Document everything** - Future you will thank you

---

**Begin Phase 1: Discovery**

