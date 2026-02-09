# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview

This is an **Agent OS** project - a structured framework for feature development using Claude Code skills and specialized subagents. Agent OS provides a standardized workflow for planning, specifying, and implementing features while maintaining consistency with user-defined coding standards.

## Agent OS Configuration

**Config Location:** `agent-os/config.yml`

Current settings:
- **Profile:** default
- **Claude Code Commands:** Enabled (Skills available as `/command-name`)
- **Claude Code Subagents:** Enabled (Implementation uses specialized subagents)
- **Version:** 2.1.1

To modify settings, run `~/agent-os/scripts/project-update.sh`

## Development Workflow

Agent OS follows a structured multi-phase workflow for feature development:

### 1. Product Planning (Optional)
**Skill:** `/plan-product`

Creates foundational product documentation:
- `agent-os/product/mission.md` - Product vision and strategy
- `agent-os/product/roadmap.md` - Phased development plan
- `agent-os/product/tech-stack.md` - Technical stack choices

### 2. Spec Shaping
**Skill:** `/shape-spec`

Initializes a new spec and gathers requirements:
- Creates dated spec folder: `agent-os/specs/YYYY-MM-DD-spec-name/`
- Uses **spec-initializer** subagent to create structure
- Uses **spec-shaper** subagent to research requirements through interactive questions
- Stores visuals in `planning/visuals/` if provided
- Creates `planning/requirements.md` with gathered requirements

### 3. Spec Writing
**Skill:** `/write-spec`

Creates formal specification document:
- Uses **spec-writer** subagent
- Creates `spec.md` from requirements and visuals
- Produces comprehensive feature specification

### 4. Task List Creation
**Skill:** `/create-tasks`

Breaks down spec into actionable tasks:
- Uses **tasks-list-creator** subagent
- Creates `tasks.md` with strategic grouping and ordering
- Tasks organized into task groups with parent/sub-task structure
- Ensures alignment with standards in `agent-os/standards/`

### 5. Implementation

Two approaches available:

**Simple Approach - `/implement-tasks`:**
- Uses **implementer** subagent directly
- Implements specified task group(s) from tasks.md
- Updates tasks.md with checkboxes `- [x]` as tasks complete
- Uses **implementation-verifier** for final verification report

**Advanced Approach - `/orchestrate-tasks`:**
- Creates `orchestration.yml` for task group management
- Allows assignment of different subagents to different task groups
- Allows selective application of standards per task group
- Coordinates multiple subagents for complex implementations

## Directory Structure

```
agent-os/
├── config.yml                    # Agent OS configuration
├── product/                      # Product-level documentation (created by /plan-product)
│   ├── mission.md
│   ├── roadmap.md
│   └── tech-stack.md
├── specs/                        # Feature specifications (created by workflow)
│   └── YYYY-MM-DD-spec-name/
│       ├── planning/
│       │   ├── requirements.md
│       │   └── visuals/
│       ├── spec.md
│       ├── tasks.md
│       ├── orchestration.yml     # Optional, for /orchestrate-tasks
│       └── verification/
│           ├── screenshots/
│           └── final-verification.md
└── standards/                    # User coding standards & preferences
    ├── global/                   # Cross-cutting standards
    │   ├── coding-style.md
    │   ├── conventions.md
    │   ├── commenting.md
    │   ├── error-handling.md
    │   ├── tech-stack.md
    │   └── validation.md
    ├── frontend/                 # Frontend-specific standards
    │   ├── accessibility.md
    │   ├── components.md
    │   ├── css.md
    │   └── responsive.md
    ├── backend/                  # Backend-specific standards
    │   ├── api.md
    │   ├── migrations.md
    │   ├── models.md
    │   └── queries.md
    └── testing/
        └── test-writing.md

.claude/
├── agents/agent-os/              # Subagent definitions
│   ├── implementer.md
│   ├── product-planner.md
│   ├── spec-initializer.md
│   ├── spec-shaper.md
│   ├── spec-writer.md
│   ├── tasks-list-creator.md
│   ├── spec-verifier.md
│   └── implementation-verifier.md
└── commands/agent-os/            # Skill definitions
    ├── plan-product.md
    ├── shape-spec.md
    ├── write-spec.md
    ├── create-tasks.md
    ├── implement-tasks.md
    └── orchestrate-tasks.md
```

## Specialized Subagents

The framework uses specialized subagents for different phases:

- **spec-initializer:** Creates new spec folder structure
- **spec-shaper:** Interactive requirements gathering through questions
- **spec-writer:** Creates formal spec.md from requirements
- **tasks-list-creator:** Breaks spec into strategic task groups
- **implementer:** Full-stack developer for feature implementation
- **spec-verifier:** Validates spec completeness
- **implementation-verifier:** End-to-end verification with screenshots
- **product-planner:** Product-level planning and documentation

## Standards System

All implementation work must align with standards defined in `agent-os/standards/`:

**Global Standards** (apply to all code):
- Consistent naming conventions and code formatting
- DRY principle, meaningful names, small focused functions
- No backward compatibility unless required
- Clear commit messages, environment configuration
- User-friendly error messages, fail fast, centralized error handling
- Minimal testing during development, focus on core user flows first

**Frontend Standards:**
- Component structure, CSS conventions, accessibility, responsive design

**Backend Standards:**
- API design, data models, database queries, migrations

**Testing Standards:**
- Write minimal tests during development
- Test only core user flows
- Defer edge case testing unless business-critical

### Standards Application in Orchestration

When using `/orchestrate-tasks`, standards can be selectively applied per task group:
- `all` - All standards files
- `global/*` - All global standards
- `frontend/*` - All frontend standards
- `backend/api.md` - Specific file
- `none` - No standards for this task group

## Key Implementation Principles

From the standards files:

1. **Code Quality:**
   - Remove dead code completely (no commented blocks)
   - No backwards-compatibility hacks unless required
   - Avoid over-engineering - solve the current problem, not hypothetical futures
   - Delete unused code rather than leaving it

2. **Error Handling:**
   - Fail fast with clear messages
   - Centralized error handling at boundaries
   - Graceful degradation for non-critical failures

3. **Testing Philosophy:**
   - Write minimal tests during feature development
   - Focus on core user flows only
   - Defer edge cases and validation testing
   - Test behavior, not implementation

4. **Implementation Workflow:**
   - Analyze existing codebase patterns first
   - Follow spec.md, requirements.md, and tasks.md exactly
   - Check off tasks in tasks.md as completed: `- [x]`
   - For UI work: Take screenshots in `verification/screenshots/`

## Common Operations

Since this is not yet a working codebase, there are no build/test/lint commands yet. These will be defined in the tech stack as features are implemented.

## Important Notes

- This repository uses Agent OS 2.1.1 with Claude Code integration
- All feature work should follow the Agent OS workflow (not ad-hoc changes)
- Standards files in `agent-os/standards/` define user preferences - always comply with these
- The orchestration system allows fine-grained control over which subagents and standards apply to which task groups
- Specs are timestamped (YYYY-MM-DD-spec-name) for versioning and tracking
