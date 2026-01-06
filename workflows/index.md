---
layout: default
title: Workflows
description: Structured execution templates for specific task types
---

# 🔄 Workflows

Structured execution templates that guide agents through specific task types. Each workflow enforces a rigorous, repeatable process.

---

## Available Workflows

<div class="grid">
  <div class="card">
    <h3><span class="card-icon">🔨</span> Build</h3>
    <p><strong>Purpose:</strong> Feature development & system enhancement</p>
    <p><strong>When to Use:</strong> Creating new features, refactoring, planned improvements</p>
    <p style="margin-top: auto; padding-top: 1rem;">
      <a href="{{ '/workflows/build.html' | relative_url }}" class="btn btn-primary">View Build Workflow →</a>
    </p>
  </div>
  
  <div class="card">
    <h3><span class="card-icon">🔍</span> Diagnose</h3>
    <p><strong>Purpose:</strong> Root cause analysis & remediation</p>
    <p><strong>When to Use:</strong> Persistent bugs, system failures, complex issues</p>
    <p style="margin-top: auto; padding-top: 1rem;">
      <a href="{{ '/workflows/diagnose.html' | relative_url }}" class="btn btn-primary">View Diagnose Workflow →</a>
    </p>
  </div>
  
  <div class="card">
    <h3><span class="card-icon">🔄</span> Migrate</h3>
    <p><strong>Purpose:</strong> Data migration & system transformation</p>
    <p><strong>When to Use:</strong> Database migrations, schema changes, data transformations</p>
    <p style="margin-top: auto; padding-top: 1rem;">
      <a href="{{ '/workflows/migrate.html' | relative_url }}" class="btn btn-primary">View Migrate Workflow →</a>
    </p>
  </div>
  
  <div class="card">
    <h3><span class="card-icon">📈</span> Evolve</h3>
    <p><strong>Purpose:</strong> Framework improvement & learning capture</p>
    <p><strong>When to Use:</strong> End of session to improve the framework itself</p>
    <p style="margin-top: auto; padding-top: 1rem;">
      <a href="{{ '/workflows/evolve.html' | relative_url }}" class="btn btn-primary">View Evolve Workflow →</a>
    </p>
  </div>
</div>

---

## Workflow Overview

<table>
  <thead>
    <tr>
      <th>Workflow</th>
      <th>Purpose</th>
      <th>When to Use</th>
      <th>Link</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><strong>🔨 build</strong></td>
      <td>Feature development & system enhancement</td>
      <td>Creating new features, refactoring, planned improvements</td>
      <td><a href="{{ '/workflows/build.html' | relative_url }}">View →</a></td>
    </tr>
    <tr>
      <td><strong>🔍 diagnose</strong></td>
      <td>Root cause analysis & remediation</td>
      <td>Persistent bugs, system failures, complex issues</td>
      <td><a href="{{ '/workflows/diagnose.html' | relative_url }}">View →</a></td>
    </tr>
    <tr>
      <td><strong>🔄 migrate</strong></td>
      <td>Data migration & system transformation</td>
      <td>Database migrations, schema changes, data transformations</td>
      <td><a href="{{ '/workflows/migrate.html' | relative_url }}">View →</a></td>
    </tr>
    <tr>
      <td><strong>📈 evolve</strong></td>
      <td>Framework improvement & learning capture</td>
      <td>End of session to improve the framework itself</td>
      <td><a href="{{ '/workflows/evolve.html' | relative_url }}">View →</a></td>
    </tr>
  </tbody>
</table>

---

## Status Indicators

Each workflow uses status indicators to communicate progress:

- `✅` - Objective completed successfully
- `⚠️` - Issue encountered and resolved autonomously
- `🚧` - Blocked, requires human input
- `🔍` - Investigation in progress

---

## How to Use Workflows

1. **Choose the Right Workflow** - Select the workflow that matches your task type
2. **Copy the Workflow** - Open the workflow file and copy its contents
3. **Customize** - Replace the mission placeholder with your specific goal
4. **Add Modifiers (Optional)** - Append behavior modifiers if needed
5. **Paste and Execute** - Paste into your chat and observe structured execution

---

## Workflow Execution Model

Every workflow follows a structured execution model:

1. **Discovery Phase** - Non-destructive investigation of current state
2. **Strategy Phase** - Planning with risk assessment and dependency mapping
3. **Execution Phase** - Autonomous implementation with continuous verification
4. **Validation Phase** - Comprehensive testing and system consistency checks
5. **Documentation Phase** - Update docs, clean workspace, report findings

Each phase must complete before proceeding. Blockers are escalated immediately with specific questions.

---

<div class="hero" style="margin-top: 3rem;">
  <h3 style="margin-top: 0;">Ready to Get Started?</h3>
  <p style="margin-bottom: 2rem; color: var(--text-secondary); font-size: 1.125rem; line-height: 1.8; max-width: 600px; margin-left: auto; margin-right: auto;">
    Choose a workflow above and start transforming your AI agent interactions with systematic, evidence-driven processes.
  </p>
  <a href="{{ '/manifest.html' | relative_url }}" class="btn btn-primary">Install Manifest First →</a>
</div>

