# Platform Engineering Workshop

A comprehensive 1-day workshop designed for Red Hat OpenShift customers to learn and implement Platform Engineering approaches customized for OpenShift running in their datacenter.

## Overview

This workshop brings together technical leaders, architects, engineers from OpenShift teams, and app dev teams to collaboratively design their internal developer platform. Through a combination of presentations and interactive activities, participants will create actionable deliverables they can immediately implement in their organizations.

**Duration:** 8 hours (9:00 AM - 5:00 PM)
**Format:** In-person, highly interactive with movement-based activities
**Participants:** 10-20 technical leaders, architects, and engineers

## Workshop Outcomes

Participants will create three key deliverables:

1. **OKRs and Goals** - Measurable objectives and key results for the year
2. **Platform Requirements** - Action items for what the platform needs to enable dev team productivity
3. **Internal Marketing Strategy** - Approach for broadcasting and promoting platform capabilities

## Workshop Topics

- Platform Engineering Fundamentals
- Team Topologies and Enabling Teams
- Developer Experience and Golden Paths
- Red Hat Developer Hub (Backstage)
- The Flywheel Effect
- Value Stream Alignment
- Self-Service Capabilities
- Metrics and Observability
- Security, Compliance, and Policy-as-Code

## Documentation

### For Participants

- **[Participant Agenda](docs/participant-agenda.md)** - Clean 2-page agenda with session times and descriptions

### For Facilitators

Complete facilitation guides for delivering the workshop:

- **[Complete Facilitator Guide](docs/facilitator-guide-complete.md)** - Master reference with table of contents, quick reference, and complete workshop flow
- **[Workshop Structure](docs/workshop-structure.md)** - 8-hour schedule design, content flow, and participant experience arc
- **[Core Sessions Facilitation Guide](docs/facilitation-guide-core-sessions.md)** - Detailed instructions for all presentation blocks and transitions
- **[Interactive Activities Guide](docs/facilitation-guide-activities.md)** - Facilitation guides for all four major activities (Future-State Visioning, OKRs, Platform Requirements, Marketing Strategy)
- **[Room Setup and Materials Guide](docs/facilitation-guide-room-materials.md)** - Physical environment configuration and comprehensive materials checklists
- **[Output Capture Guide](docs/output-capture-guide.md)** - Photography, documentation, and post-workshop deliverables creation

## Getting Started

### For Facilitators

1. **4 Weeks Before:** Review the [Complete Facilitator Guide](docs/facilitator-guide-complete.md) and [Workshop Structure](docs/workshop-structure.md)
2. **2 Weeks Before:** Order materials using the checklist in the [Room Setup and Materials Guide](docs/facilitation-guide-room-materials.md)
3. **1 Week Before:** Review all session-specific guides and prepare presentations
4. **Day Before:** Set up room using guidance in [Room Setup and Materials Guide](docs/facilitation-guide-room-materials.md)
5. **Workshop Day:** Use [Complete Facilitator Guide](docs/facilitator-guide-complete.md) as your primary reference
6. **Post-Workshop:** Follow [Output Capture Guide](docs/output-capture-guide.md) to create participant deliverables

### For Participants

Review the [Participant Agenda](docs/participant-agenda.md) before attending to understand the workshop flow and what to bring.

## Workshop Activities

### 1. Future-State Visioning Exercise (9:00 AM - 9:50 AM)
Creative exercise where participants envision their organization's future success with platform engineering, using the "DAANG!" headline format to inspire aspirational thinking.

### 2. OKRs and Goals Development (1:00 PM - 2:00 PM)
Small group activity to develop specific, measurable objectives and key results for platform engineering initiatives.

### 3. Platform Requirements Gathering (3:30 PM - 4:30 PM)
High-energy standing wall exercise using post-it notes to identify pain points, desired capabilities, and priorities through affinity mapping.

### 4. Marketing Strategy Development (Optional Extension)
Can be used as extended workshop, follow-up session, or takeaway assignment for developing stakeholder communication strategies.

## Materials Needed

Key materials for the workshop:
- Post-it notes (3x3 inch, multiple colors)
- Flip chart stands and paper
- Markers (thick for flip charts, fine-tip for post-its)
- Masking tape or painter's tape
- Projector and screen
- Camera/tablet for photo documentation

See the [Room Setup and Materials Guide](docs/facilitation-guide-room-materials.md) for complete materials checklist organized by session.

## Project Structure

```
PlatformEngineering/
├── README.md                          # This file
├── CLAUDE.md                          # Guidance for AI assistants
├── docs/                              # Workshop documentation
│   ├── workshop-structure.md
│   ├── participant-agenda.md
│   ├── facilitation-guide-complete.md
│   ├── facilitation-guide-core-sessions.md
│   ├── facilitation-guide-activities.md
│   ├── facilitation-guide-room-materials.md
│   └── output-capture-guide.md
├── agent-os/                          # Agent OS framework
│   ├── product/                       # Product planning
│   │   ├── mission.md
│   │   ├── roadmap.md
│   │   └── tech-stack.md
│   ├── specs/                         # Feature specifications
│   │   └── 2026-02-09-workshop-agenda-facilitation-guide/
│   └── standards/                     # Coding standards
└── .claude/                           # Claude Code configuration
```

## Technical Details

This project uses the Agent OS framework with Claude Code for structured feature development. The workshop materials were created through a systematic workflow:

1. Product Planning - Mission, roadmap, and tech stack
2. Spec Shaping - Requirements gathering with visual analysis
3. Spec Writing - Formal specification creation
4. Task List Creation - Strategic breakdown into task groups
5. Implementation - Six task groups executed sequentially
6. Verification - Final verification report

See [CLAUDE.md](CLAUDE.md) for details on the Agent OS framework and development workflow.

## License and Usage

This workshop is designed for Red Hat OpenShift customers and partners. Materials are customized for OpenShift environments running in customer datacenters.

## Contributing

To modify or extend the workshop materials, follow the Agent OS workflow documented in [CLAUDE.md](CLAUDE.md). Use the `/shape-spec`, `/write-spec`, `/create-tasks`, and `/implement-tasks` commands to create new features or modifications.

## Support

For questions about the workshop content or facilitation, refer to the troubleshooting sections in:
- [Complete Facilitator Guide](docs/facilitator-guide-complete.md) - Section 8: Troubleshooting Common Challenges
- [Room Setup and Materials Guide](docs/facilitation-guide-room-materials.md) - Troubleshooting sections throughout

---

**Total Documentation:** 9,214 lines across 7 comprehensive guides
**Status:** Production Ready ✅
**Last Updated:** February 2026
