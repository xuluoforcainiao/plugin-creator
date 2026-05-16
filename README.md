# QoderWork Plugin Creator

Create, customize, or modify QoderWork expert plugins. A plugin is NOT a single skill — it is a role/industry-oriented toolkit that packages the major tasks of a specific role into a unified, manageable suite.

## Key Concepts

- **Plugin**: A role-oriented toolkit. For example, "Legal Assistant" contains contract drafting, review, legal research, compliance check, etc.
- **Skill**: A single capability within a plugin. Each Skill handles one specific task.
- **MCP**: A bridge between AI and external tools (DingTalk, Slack, Notion, etc.)

## Creation Workflow

### Step 1: Understand User's Role
Clarify role, main tasks, pain points, platforms used.

### Step 2: Plan Skill Structure
List Skills to create, get user confirmation.

### Step 3: Collect Reference Materials (Critical)
Gather templates, SOPs, good examples, checklists, reference docs. This determines plugin quality.

### Step 4: Build the Plugin
Directory structure:

```
{plugin-name}/
├── .qoder-plugin/
│   └── plugin.json          # Plugin metadata
├── skills/
│   ├── skill-a/
│   │   ├── SKILL.md
│   │   └── references/      # Reference materials
│   └── skill-b/
│       └── SKILL.md
└── README.md
```

### Step 5: Post-Creation Guidance
Explain how to invoke and that the plugin can evolve over time.

## Two Plugin Modes

| Mode | Use Case | Structure |
|------|---------|-----------|
| Simple Tool Mode | Skills are independent | Skills under skills/ |
| Orchestration Mode | Multi-stage with dependencies | Add orchestrator Skill |

## Best Practices

1. Use descriptive kebab-case naming
2. Provide bilingual descriptions
3. Focus on a specific industry scenario
4. Single responsibility per Skill
5. Use references/ for templates and examples
6. Write a README explaining use cases

## Version

Current: v1.4.0
