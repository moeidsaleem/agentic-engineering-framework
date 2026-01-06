---
layout: default
title: Troubleshooting Guide
description: Common issues and solutions for the Agentic Engineering Framework - fix agent behavior problems, workflow issues, and Cursor AI integration challenges
keywords: Cursor AI troubleshooting, AI framework issues, agent behavior problems, workflow fixes, AI agent debugging
---

# Troubleshooting Guide

**Author:** Moeid Saleem Khan  
**Version:** 2.0

Common issues and solutions when using the framework.

---

## Agent Not Following Workflow

**Symptoms:**
- Agent skips phases
- Agent doesn't provide status markers
- Agent doesn't follow structured format

**Solutions:**
1. **Verify Manifest Installation**
   - Check that `manifest.md` is properly installed in Cursor rules
   - Ensure it's the active rule set (not overridden)
   - Try reinstalling the manifest

2. **Check Workflow Format**
   - Ensure you copied the entire workflow
   - Verify the mission placeholder was replaced
   - Check that modifiers (if used) are properly appended

3. **Explicit Reminder**
   - Add: "Follow the workflow phases exactly as specified"
   - Reference the specific workflow file name

---

## Agent Claims "File Not Found"

**Symptoms:**
- Agent says file doesn't exist
- Agent stops searching after first attempt
- You know the file exists

**Solutions:**
1. **Remind Agent of Search Protocol**
   - "Use exhaustive search protocol from manifest"
   - "Search recursively with **/pattern"
   - "Check subdirectories you may have skipped"

2. **Provide Context**
   - "The file is in the project root or a subdirectory"
   - "It might have a different extension"
   - "Check related directories"

3. **Escalate if Needed**
   - "My search was insufficient. Escalating to full directory scan."

---

## Agent Making Assumptions

**Symptoms:**
- Agent proceeds without investigation
- Agent trusts documentation over code
- Agent doesn't verify before changing

**Solutions:**
1. **Enforce Investigation Protocol**
   - "Follow the Investigation Protocol from manifest"
   - "Verify against actual code, not documentation"
   - "Map system architecture before proceeding"

2. **Explicit Instructions**
   - "Investigate first, then report findings"
   - "Trust code over docs - verify everything"
   - "Show me the actual code before making changes"

---

## Agent Not Completing Task Chains

**Symptoms:**
- Agent fixes one issue, stops
- Agent doesn't fix related problems
- Agent marks complete with issues remaining

**Solutions:**
1. **Remind of Complete Task Chains Principle**
   - "Fix entire problem sets, not just symptoms"
   - "If Task A reveals Issue B, fix both"
   - "Complete task chains before marking done"

2. **Explicit Scope**
   - "Fix all related issues, not just this one"
   - "Check for similar patterns elsewhere"
   - "Ensure system consistency"

---

## Agent Asking for Permission Unnecessarily

**Symptoms:**
- Agent asks before executing clear tasks
- Agent escalates when it should proceed
- Agent requests confirmation for autonomous actions

**Solutions:**
1. **Remind of Autonomous Execution**
   - "Proceed autonomously after research"
   - "Execute within guardrails, escalate only when blocked"
   - "Default to action, not permission"

2. **Clarify Escalation Triggers**
   - "Only escalate for: ambiguous requirements, multiple valid approaches, security concerns, missing critical info"
   - "This is clear - proceed"

---

## Agent Not Updating Documentation

**Symptoms:**
- Documentation remains outdated
- Agent doesn't update docs after changes
- Agent creates duplicate docs instead of updating

**Solutions:**
1. **Explicit Documentation Requirement**
   - "Update documentation to reflect changes"
   - "Update existing docs, don't create duplicates"
   - "Keep documentation current with code"

2. **Specify What to Update**
   - "Update README.md with new API endpoint"
   - "Update docs/auth.md with implementation details"
   - "Update inline comments if behavior changed"

---

## Agent Using Wrong Tools

**Symptoms:**
- Agent uses bash for file operations
- Agent uses file tools for system commands
- Agent doesn't use absolute paths

**Solutions:**
1. **Remind Tool Usage Rules**
   - "Use file tools for file operations, bash for system commands"
   - "Use absolute paths for file operations"
   - "Read manifest section on Tool & Command Execution"

2. **Correct Tool Selection**
   - "Use file read tool, not cat"
   - "Use file edit tool, not sed"
   - "Use absolute paths"

---

## Agent Not Testing Continuously

**Symptoms:**
- Agent waits until end to test
- Agent doesn't verify after changes
- Agent marks complete without testing

**Solutions:**
1. **Enforce Continuous Verification**
   - "Test after each significant change"
   - "Run tests and lints immediately"
   - "Verify before marking complete"

2. **Explicit Testing Requirements**
   - "Run tests after this change"
   - "Verify integration points work"
   - "Check for regressions"

---

## Agent Creating Unnecessary Files

**Symptoms:**
- Agent creates temp files and doesn't clean up
- Agent creates duplicate documentation
- Agent leaves debug files

**Solutions:**
1. **Remind Cleanup Requirements**
   - "Clean up temp files when done"
   - "Use designated temp directories"
   - "Remove debug code and console.logs"

2. **Explicit Cleanup**
   - "Clean workspace before marking complete"
   - "Remove temp files in tmp/ directory"
   - "Delete debug scripts"

---

## Agent Not Using Existing Tools

**Symptoms:**
- Agent recreates existing scripts
- Agent doesn't check scripts/ directory
- Agent builds one-off solutions

**Solutions:**
1. **Remind Reusability Principle**
   - "Check scripts/ directory first"
   - "Use existing tools before creating new"
   - "Build for reuse, not one-off"

2. **Point to Existing Tools**
   - "Check scripts/api-wrappers/ for existing API tool"
   - "Use scripts/database/backup.sh instead of creating new"

---

## Workflow Not Producing Expected Results

**Symptoms:**
- Workflow seems too verbose
- Workflow seems too brief
- Workflow doesn't match your needs

**Solutions:**
1. **Use Modifiers**
   - Append `modifiers/terse.md` for concise output
   - Append `modifiers/professional.md` for formal tone

2. **Customize Workflow**
   - Adapt workflow templates for your domain
   - Maintain core execution model
   - Customize phases as needed

3. **Provide Feedback**
   - Use `workflows/evolve.md` to capture what didn't work
   - Propose improvements to the framework

---

## General Debugging Tips

1. **Check Manifest Installation**
   - Is it active?
   - Is it complete?
   - Is it the latest version?

2. **Verify Workflow Format**
   - Complete workflow copied?
   - Mission placeholder replaced?
   - Modifiers properly appended?

3. **Review Agent Output**
   - Does it follow phases?
   - Does it provide status markers?
   - Does it follow structured format?

4. **Escalate When Needed**
   - If agent is truly stuck, provide specific guidance
   - Reference specific sections of manifest
   - Provide examples of desired behavior

---

## Getting Help

If issues persist:
1. Review the manifest section relevant to your issue
2. Check examples in `examples/` directory
3. Use `workflows/evolve.md` to document the issue
4. Consider customizing the framework for your specific needs

---

**Remember: The framework is designed to be adapted. Customize it for your environment while maintaining core principles.**

