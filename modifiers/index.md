---
layout: default
title: Behavior Modifiers
description: Optional behavior modifiers for the Agentic Engineering Framework - terse communication and professional language adjustments for AI agents
keywords: AI behavior modifiers, Cursor AI modifiers, AI communication styles, AI agent customization
---

# 🎛️ Behavior Modifiers

Optional, stackable behavior adjustments that can be appended to workflows for specific communication styles or operational modes.

---

## Available Modifiers

<div class="grid">
  <div class="card">
    <h3><span class="card-icon">⚡</span> Terse</h3>
    <p><strong>Purpose:</strong> Ultra-concise, information-dense communication</p>
    <p><strong>Effect:</strong> Removes all conversational filler, pleasantries, and redundant explanations. Every word carries information.</p>
    <p style="margin-top: auto; padding-top: 1rem;">
      <a href="{{ '/modifiers/terse.html' | relative_url }}" class="btn btn-primary">View Terse Modifier →</a>
    </p>
  </div>
  
  <div class="card">
    <h3><span class="card-icon">💼</span> Professional</h3>
    <p><strong>Purpose:</strong> Eliminates sycophantic language and filler</p>
    <p><strong>Effect:</strong> Removes phrases like "You're absolutely right!" and focuses on brief, factual acknowledgments only.</p>
    <p style="margin-top: auto; padding-top: 1rem;">
      <a href="{{ '/modifiers/professional.html' | relative_url }}" class="btn btn-primary">View Professional Modifier →</a>
    </p>
  </div>
</div>

---

## How to Use Modifiers

### Stacking Modifiers

You can combine multiple modifiers for specific scenarios:

```markdown
[workflow content]
---
[modifier 1 content]
---
[modifier 2 content]
```

### Example Usage

1. **Copy your workflow** (e.g., `workflows/build.md`)
2. **Append modifier content** at the bottom
3. **Paste into chat** - The agent will follow both the workflow and modifier instructions

### When to Use

- **Terse Modifier:** When you need fast, information-dense communication
- **Professional Modifier:** When you want formal, technical communication without flattery
- **Both Together:** For maximum efficiency and professionalism

---

## Modifier Overview

<table>
  <thead>
    <tr>
      <th>Modifier</th>
      <th>Effect</th>
      <th>Link</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><strong>⚡ terse</strong></td>
      <td>Ultra-concise, information-dense communication</td>
      <td><a href="{{ '/modifiers/terse.html' | relative_url }}">View →</a></td>
    </tr>
    <tr>
      <td><strong>💼 professional</strong></td>
      <td>Eliminates sycophantic language and filler</td>
      <td><a href="{{ '/modifiers/professional.html' | relative_url }}">View →</a></td>
    </tr>
  </tbody>
</table>

---

<div class="hero" style="margin-top: 3rem;">
  <h3 style="margin-top: 0;">Ready to Customize Your AI Agent?</h3>
  <p style="margin-bottom: 2rem; color: var(--text-secondary); font-size: 1.125rem; line-height: 1.8; max-width: 600px; margin-left: auto; margin-right: auto;">
    Use modifiers to tailor your AI agent's communication style to your preferences.
  </p>
  <a href="{{ '/workflows/' | relative_url }}" class="btn btn-primary">View Workflows →</a>
</div>

