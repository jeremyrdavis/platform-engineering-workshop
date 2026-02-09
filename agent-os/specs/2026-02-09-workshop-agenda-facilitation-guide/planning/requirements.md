# Spec Requirements: Workshop Agenda and Facilitation Guide

## Initial Description
This is for creating a comprehensive agenda and facilitation guide for a 1-day in-person Platform Engineering workshop delivered to Red Hat OpenShift customers.

## Requirements Discussion

### First Round Questions

**Q1:** I assume the workshop should run from approximately 8:30 AM to 5:00 PM with registration/breakfast at 8:30 AM, formal start at 9:00 AM, lunch break around noon, and wrap-up by 5:00 PM. Is that correct, or do you have a different timeframe in mind?

**Answer:** 9:00 AM to 5:00 PM (8 hours)

**Q2:** I'm thinking the agenda should alternate between presentations (15-30 minutes each) and interactive activities (30-60 minutes each) to maintain energy and engagement. Should we aim for roughly 40% presentation time and 60% interactive activity time, or a different balance?

**Answer:** Start the day with presentations to introduce the concepts. A Developer Hub presentation could be moved later in the day. (So foundational concepts first, then activities, with Developer Hub as a mid-day topic)

**Q3:** For the facilitation guide, I assume you want detailed facilitator notes including exact timing, transition scripts, discussion prompts, what to write on whiteboards, how to distribute post-it notes, and troubleshooting tips for each session. Is that the level of detail you're looking for?

**Answer:** Yes - detailed facilitator notes including exact timing, transition scripts, discussion prompts, what to write on whiteboards, how to distribute post-it notes, and troubleshooting tips for each session.

**Q4:** I'm thinking the participant-facing agenda should be a clean 1-2 page document showing session titles, times, and brief descriptions, while the facilitator guide would be a much more detailed 20-30 page document with all the behind-the-scenes instructions. Should these be two separate deliverables?

**Answer:** Yes - participant-facing agenda should be a clean 1-2 page document, while the facilitator guide would be a detailed 20-30 page document with all behind-the-scenes instructions.

**Q5:** For the three main deliverable-creation activities (OKRs, Platform Requirements, Marketing Strategy), should these happen after relevant presentation content has been covered, or should we front-load all presentations and do all activities in the afternoon?

**Answer:** The three main deliverable-creation activities (OKRs, Platform Requirements, Marketing Strategy) should occur after the relevant concepts have been introduced in presentations. User also wants suggestions for more topics.

**Q6:** I assume we should include buffer time between sessions (5-10 minutes) for breaks, transitions, and Q&A that runs over. Should we build in explicit 15-minute breaks mid-morning and mid-afternoon, plus the lunch break?

**Answer:** Yes - build in explicit breaks (mid-morning, mid-afternoon, plus lunch)

**Q7:** For group sizing in interactive activities, I'm thinking we should plan for 20-30 participants broken into groups of 4-6 people for small group work. Is that the expected participant count and group size?

**Answer:** Closer to 10 participants with a maximum of 20 participants. Groups of 4-6 for small group work.

**Q8:** Should the agenda and facilitation guide include guidance for what to do if the workshop is adapted for virtual delivery, or should we focus exclusively on the in-person format for now?

**Answer:** Focus exclusively on in-person format for now.

### Existing Code to Reference

No similar existing features identified for reference.

## Visual Assets

### Files Provided:
- `IMG_1916.png`: Workshop room setup showing collaborative environment with participants working at tables and using windows/walls for post-it note activities
- `IMG_1918.png`: Additional angle of same workshop showing dynamic participation with both seated and standing work
- `IMG_1925.png`: Flip chart example showing workshop output - a future-state vision exercise titled "DAANG! Delta takes Facebook's spot in TECH TOP 5"

### Visual Insights:

**Workshop Environment & Setup (IMG_1916.png, IMG_1918.png):**
- Collaborative room configuration with tables supporting laptop work and small group discussions
- Extensive use of windows/walls as collaborative surfaces for post-it note exercises
- Participants actively standing and working at windows for visual brainstorming and affinity mapping
- Mix of seated table work and standing wall-based activities showing dynamic, energizing format
- Room allows simultaneous activities: some participants at tables, others at walls/windows
- Post-it notes heavily utilized for group exercises and visual organization of ideas
- Laptops present but activity-focused (not presentation-heavy)
- Natural light and open space creating engaging atmosphere

**Activity Example Output (IMG_1925.png):**
- Flip chart showing hand-written group work output
- Exercise appears to be a future-state vision or success story creation activity
- Title format: "[Company] [Achievement headline]"
- Content: Bulleted list of platform engineering outcomes and benefits achieved
- Specific outcomes shown in example:
  - Faster onboarding
  - True CI/CD
  - Multiple prod pushes per day
  - Roll forward, not back
  - Open source contributions
  - Industry publications
  - Competitive pay & work schedules
  - Self-service developer products
  - Standardized frameworks
- This suggests a creative visioning exercise where participants imagine their organization's future success with platform engineering

**Key Design Patterns Identified:**
- Active, movement-based activities (not just seated discussions)
- Visual collaboration using post-it notes on large surfaces
- Mix of analog (flip charts, post-its) and digital (laptops) tools
- Group outputs captured on flip charts for sharing
- Future-state visioning as a motivational/goal-setting technique
- Success story framework for articulating platform engineering value

**Fidelity Level:**
These are photographs of an actual workshop in progress, showing real-world implementation of the workshop format and activities.

## Requirements Summary

### Functional Requirements

**Workshop Structure:**
- Full-day in-person workshop running 9:00 AM to 5:00 PM (8 hours total)
- Target audience: Technical leaders, architects, engineers from OpenShift teams, and app dev teams
- Expected participants: 10-20 attendees (optimal: 10, maximum: 20)
- Small group activities with breakout groups of 4-6 people

**Content Flow:**
- Begin with foundational presentation content to introduce concepts
- Intersperse interactive activities after relevant concepts have been presented
- Developer Hub presentation positioned as mid-day topic
- Three major deliverable-creation activities positioned strategically throughout the day:
  - OKRs/goals for the year
  - Action Items for platform needs
  - Approach for broadcasting/marketing platform updates

**Core Topics to Cover:**
- Platform engineering principles and the flywheel effect
- Value stream alignment and business impact
- Platform team structures and enabling teams
- Developer experience and internal developer platforms
- Backstage/Red Hat Developer Hub
- Onboarding applications and app dev teams
- Golden paths and self-service capabilities
- Metrics, observability, and DORA metrics
- Security, compliance, and policy-as-code
- Internal marketing and communication strategies
- OKR development for platform teams
- Cross-functional collaboration patterns
- Organizational change management and adoption strategies

**Scheduling Requirements:**
- Explicit breaks: mid-morning break, lunch break, mid-afternoon break
- Buffer time between sessions for transitions and Q&A overflow
- Balance between presentation time and interactive activity time with presentations front-loaded

**Deliverables to Create:**

1. **Participant-Facing Agenda (1-2 pages):**
   - Clean, simple document
   - Session titles with times
   - Brief descriptions of each session
   - Break times clearly marked
   - Format: Markdown (exportable to PDF)

2. **Facilitator Guide (20-30 pages):**
   - Detailed facilitator notes for every session
   - Exact timing for each segment
   - Transition scripts between sessions
   - Discussion prompts and question banks
   - Whiteboard/flip chart preparation instructions (what to write, when)
   - Physical materials distribution guidance (post-it notes, markers, handouts)
   - Room setup instructions for different activity types
   - Instructions for transitioning between seated and standing activities
   - Guidance for wall/window-based post-it note exercises
   - Affinity mapping and visual brainstorming facilitation techniques
   - Troubleshooting tips for common challenges
   - Group formation and management instructions
   - Setup requirements for each activity
   - Expected outputs for each interactive session
   - Photo capture guidance for documenting flip chart and post-it outputs
   - Format: Markdown (exportable to PDF)

**Workshop Outputs (Created by Participants):**
- OKRs and goals for the platform team's year
- Prioritized action items for platform needs and improvements
- Strategy and approach for broadcasting/marketing platform updates internally
- Future-state vision/success stories (based on visual example showing desired platform engineering outcomes)

**Interactive Activity Formats (Based on Visual Evidence):**
- Post-it note exercises on windows/walls for brainstorming and affinity mapping
- Flip chart group work for capturing shared outputs
- Future-state visioning exercise (creating success story headlines and outcome lists)
- Mix of seated small group discussions and standing collaborative wall work
- Visual organization and clustering of ideas using post-it notes
- Group sharing and gallery walks to review other teams' outputs

**Technical Delivery Requirements:**
- Physical materials: Post-it notes (multiple colors), whiteboards/flip charts, markers, masking tape/painter's tape
- Timing tools: Timer/clock for session management
- Optional: OpenShift Dev Spaces and Developer Hub for demonstrations (no hands-on labs)
- Digital camera or smartphone for capturing flip chart and post-it outputs
- Templates and worksheets for participant exercises
- Wall/window space for post-it note activities
- Flip chart stands and paper pads

**Additional Topics Requested:**
User has requested suggestions for additional workshop topics beyond the core topics listed above.

**Activity Design Principles (Derived from Visuals):**
- Encourage movement and physical engagement (standing activities at walls)
- Use visual collaboration techniques (post-it notes, flip charts)
- Create tangible outputs that can be photographed and shared
- Mix individual reflection, small group work, and full group sharing
- Use creative/aspirational exercises (future-state visioning) to energize and motivate
- Provide clear frameworks for capturing ideas (bullet lists, headline formats)
- Make outputs visible to entire group (flip charts, wall displays)

### Reusability Opportunities

No existing components, templates, or similar features identified for reuse. This will be a greenfield creation of workshop materials.

However, the visual assets show a proven workshop format and activity structure that should be replicated in the agenda and facilitation guide.

### Scope Boundaries

**In Scope:**
- Comprehensive 1-day workshop agenda with exact timing
- Detailed facilitator guide with scripts, prompts, and instructions
- Participant-facing agenda document (1-2 pages)
- Session descriptions for all presentations and activities
- Instructions for three major deliverable-creation activities
- Instructions for future-state visioning exercise (based on visual example)
- Room setup and configuration guidance for different activity types
- Post-it note exercise facilitation instructions
- Flip chart activity guidance
- Affinity mapping and visual brainstorming techniques
- Photo documentation guidance for capturing outputs
- Break scheduling and transition management
- Small group activity facilitation guidance
- Physical materials preparation lists
- Troubleshooting guidance for facilitators
- Suggestions for additional workshop topics
- In-person delivery format only

**Out of Scope:**
- Actual presentation slide decks (these exist separately per tech-stack.md)
- Virtual/remote delivery adaptations
- Hands-on technical labs or deployment exercises
- Post-workshop follow-up materials (email templates, resource links)
- Participant handout templates (these may be created separately)
- Detailed content for each presentation (covered in separate presentation materials)
- Multi-day workshop variations
- Workshop marketing or registration materials
- Procurement of physical materials (post-its, flip charts, etc.)

### Technical Considerations

**Content Format:**
- Primary format: Markdown for all workshop documentation
- Export capability: PDF for distribution to facilitators and participants
- Version control: Git-based management for iterations and updates

**Physical Environment Assumptions:**
- In-person venue with capacity for 10-20 participants
- Whiteboard or flip chart availability (multiple flip chart stands preferred)
- Windows or wall space suitable for post-it note activities
- Projector/screen for presentations
- Space for small group breakouts (or ability to rearrange room)
- Tables for group work with post-it notes and materials
- Room configuration allowing both seated and standing activities
- Adequate lighting for both presentation viewing and collaborative work
- Space to display multiple flip charts simultaneously for group sharing

**Facilitation Context:**
- Workshop delivered by experienced Red Hat facilitators
- Target customer: Red Hat OpenShift customers exploring platform engineering
- Mix of technical and organizational content
- Emphasis on practical, actionable outputs participants can take back to their organizations
- Interactive, engaging format to maintain energy throughout full day
- Dynamic activities requiring participant movement and active collaboration
- Visual and kinesthetic learning approaches integrated throughout
- Balance of creative visioning and concrete planning exercises

**Integration with Existing Product Materials:**
- Presentations delivered via Google Slides (existing format per tech-stack.md)
- Reference to Red Hat Developer Hub and OpenShift Dev Spaces for demonstrations
- Alignment with platform engineering principles and Red Hat's approach
- Connection to broader platform engineering community and resources

**Activity Facilitation Requirements (Based on Visual Evidence):**
- Clear instructions for setting up post-it note exercises on walls/windows
- Guidance for managing transitions between seated and standing activities
- Techniques for affinity mapping and idea clustering with post-it notes
- Instructions for facilitating group sharing of flip chart outputs
- Tips for keeping energy high during full-day workshop
- Strategies for encouraging quiet participants to engage in wall-based activities
- Methods for capturing and preserving analog outputs (photos, transcription)
