# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a documentation repository for tracking the restoration of Gemma, a 2002 BMW E46 330ci. The car was received as a non-running rusty shell and is being restored to original OEM condition. This repository uses a simple markdown-based system to track parts, work logs, and progress.

**Vehicle Details:**
- **Model:** 2002 BMW E46 330ci (Coupe)
- **Engine:** M54B30 (3.0L inline-6, 225 HP)
- **Color:** Black
- **Condition:** Non-running for 3+ years, significant rust repair needed
- **Goal:** Full OEM restoration

## Required Expertise

When assisting with this project, you should provide expertise in:

1. **BMW E46 Mechanical Systems:**
   - M54B30 engine diagnostics, maintenance, and repair
   - Rear subframe reinforcement (common E46 issue)
   - Suspension geometry and component replacement
   - Brake system (including brake line routing)
   - Fuel system (tank, lines, pump)

2. **BMW E46 Electrical Systems:**
   - Wiring harness routing and connections
   - Engine management system (DME/ECU)
   - Sensor locations and specifications
   - Starting system diagnostics
   - Basic electrical troubleshooting

3. **Bodywork & Restoration:**
   - Rust repair techniques for floor pans
   - Welding and paint preparation
   - Undercarriage restoration
   - OEM specifications and procedures

4. **E46-Specific Knowledge:**
   - Common failure points and preventative measures
   - OEM part numbers and aftermarket alternatives
   - Torque specifications for critical components
   - Reassembly order and dependencies
   - Forum resources and technical documentation

When the user asks technical questions, provide specific E46-relevant answers including part numbers, torque specs, common issues, and recommended procedures.

## Current Restoration Plan

The restoration follows a two-phase approach:

### PLAN 0: Temporary Assembly & Workshop Setup

**Goal:** Make the car movable and get it under weather protection.

1. Install bare minimum rear suspension (temporary, just to roll)
2. Push car into position for marquee
3. Build/set up marquee (weather protection tent)
4. Remove suspension again for full access to underside

**Status:** Ready to begin

### PLAN 1: Underside Restoration (Main Work Sequence)

**Completed Work:**
- ✓ Rear floor rust sections cut out and patched
- ✓ Floor patches welded with weld-through primer applied

**Phase 1: Structural Reinforcement & Brackets**
1. Install Reddish Motorsport v3 rear subframe reinforcement plates (critical E46 weak point)
2. Remove old rusty brake and fuel tank brackets (expect seized bolts, may need cutting)
3. Install new brake and fuel tank brackets (before painting, to ensure fitment)

**Phase 2: Initial Cleaning & Assessment**
1. Clean all underside (initial degreasing, remove loose debris)
2. Wirewheel entire underside (remove loose rust, old paint, scale - get to bare metal)
3. Apply rust converter/remover (first pass - allow proper cure time)

**Phase 3: Touch-Up Welding & Repairs**
1. Weld heat shield screw holes/studs (repair stripped or rusty mounting points)
2. Repair rusty plug holes (seal any rust-through holes)
3. Repair/reinforce battery bracket area (common E46 rust spot)
4. Other touch-up welding as discovered during assessment

**Phase 4: Final Cleaning & Surface Prep**
1. Power wash entire underside (remove all welding/grinding residue)
2. Degrease thoroughly (critical for paint adhesion - must be spotless)
3. Apply rust converter/remover (final pass before primer)

**Phase 5: Paint & Protection**
1. Apply epoxy 2K primer (critical corrosion barrier)
2. Apply anti-rust chassis paint (2-3 coats, follow cure times)
3. Allow full cure time (24-72 hours per paint specifications)

**Phase 6: Disassembled Parts Restoration**
1. Strip all disassembled parts (suspension arms, subframe components, brackets)
2. Prime disassembled parts (proper surface prep first)
3. Paint disassembled parts (multiple coats, proper cure time)
4. Apply top coat to parts (optional but recommended)

### POST-UNDERSIDE: First Start Preparation

After underside restoration is complete:

1. **Reinstall wiring harness** - Document all connections with photos, test each circuit
2. **Install battery** - New battery in repaired bracket, ensure clean grounds
3. **Install basic start components** - Minimum needed: fuel system, ignition, starter circuit
4. **Attempt first start** - Engine hasn't run in 3+ years, expect troubleshooting

### Important Process Notes

**Underside Restoration Best Practices:**
- Do NOT skip the degreasing step - paint will not adhere to oily surfaces
- Allow proper cure times between rust treatment, primer, and paint
- Epoxy 2K primer is critical for long-term corrosion protection
- Multiple thin coats are better than one thick coat
- Mask/protect areas that shouldn't be painted (bearing surfaces, threaded holes)
- Safety first: respirator required for painting and rust treatment

**E46-Specific Considerations:**
- Rear subframe reinforcement (Reddish v3 plates) MUST be installed before reassembly - this is a known E46 failure point
- Battery bracket area commonly rusts - inspect and repair thoroughly
- Heat shield mounting points often corrode - repair before reassembly

When discussing the project, refer to this detailed sequence and provide advice relevant to the current phase. See `progress/current-tasks.md` for the complete checklist.

## Repository Structure

- `parts/` - Parts inventory tracking (purchased and needed parts)
- `logs/` - Chronological work logs for each work session
- `progress/` - Task tracking and milestone management
- `photos/` - Photo documentation and reference materials

## Common Tasks

### Adding a New Part

When the user wants to add a part they purchased:

1. Read `parts/purchased.md`
2. Use the Edit tool to add a new part entry following the template format
3. Include: part name, part number, supplier, date, cost, status, and notes
4. Maintain the existing formatting and structure

### Creating a Work Log

When the user wants to document work they performed:

1. Create a new file in `logs/` with the naming convention: `YYYY-MM-DD-brief-description.md`
2. Copy the template from `logs/log-template.md`
3. Fill in the relevant sections based on the user's description
4. If tasks were completed, also update `progress/current-tasks.md` and `progress/completed-tasks.md`

### Managing Tasks

When the user wants to add or update tasks:

1. For new tasks: Add to `progress/current-tasks.md` under the appropriate section (In Progress, Up Next, or Blocked)
2. For completed tasks: Move from `current-tasks.md` to `completed-tasks.md` with completion date
3. If a major milestone is reached: Update the relevant checklist in `progress/milestones.md`

### Tracking Parts Needed

When the user identifies a part they need:

1. Read `parts/needed.md`
2. Add the part under the appropriate priority section
3. Include estimated cost, potential suppliers, and any relevant notes

### Generating Reports

When the user asks for summaries or reports:

- **Cost summary**: Read all entries in `parts/purchased.md` and calculate totals
- **Progress summary**: Read `progress/milestones.md` and count completed items per phase
- **Recent work**: List the most recent log files in `logs/`
- **Time tracking**: Parse duration fields from work logs

## File Conventions

### Date Format
Always use ISO 8601 format: `YYYY-MM-DD` (e.g., `2025-11-07`)

### Log File Naming
Pattern: `YYYY-MM-DD-brief-description.md`
- Use lowercase with hyphens
- Keep descriptions concise but descriptive
- Examples: `2025-01-15-engine-disassembly.md`, `2025-02-20-rust-repair.md`

### Currency Format
Use USD with dollar sign: `$XXX.XX`

### Task Status
Use markdown checkboxes:
- `- [ ]` for incomplete tasks
- `- [x]` for completed tasks

## Markdown Standards

- Use `###` (H3) for part entries in parts lists
- Use `##` (H2) for major sections in logs and progress files
- Maintain consistent bullet point formatting
- Preserve template structures when adding entries

## Photo References

When referencing photos from work logs or other documents:
- Use relative paths: `../photos/folder/filename.jpg`
- Use markdown image syntax: `![Description](path)`
- Encourage descriptive alt text

## Workflow Philosophy

This repository prioritizes:
1. **Simplicity**: Plain markdown files that can be edited anywhere
2. **Chronology**: Date-based organization for easy tracking
3. **Completeness**: Comprehensive documentation for future reference
4. **Flexibility**: Templates are guides, not rigid requirements

## Helper Commands

When the user asks for help with common operations:

- "Add a part" → Guide to parts/purchased.md or parts/needed.md
- "Log today's work" → Create new log file with today's date
- "What's next?" → Show current-tasks.md
- "Cost so far?" → Parse and sum all costs from parts/purchased.md
- "Progress report" → Summarize completion status from milestones.md
