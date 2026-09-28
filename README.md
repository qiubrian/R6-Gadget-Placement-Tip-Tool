# R6 Gadget Placement Tool

> An unofficial, patch-aware library of verified operator placements and site-specific tactics for Rainbow Six Siege.

## Project Status

This project is currently in the research and prototype phase.

## Overview

R6 Strat Maker helps players find useful, reproducible tactics for a chosen operator on a specific map and bomb site.

Instead of recommending which operator to play, the application answers questions such as:

- Where should I place Mira’s Black Mirrors on this site?
- Which walls or hatches can one Kaid Electroclaw cover?
- Where can Fuze safely deploy Cluster Charges?
- What paths should Ram use to create useful vertical pressure?
- Where should Zero cameras be fired?
- Which C4, grenade, or gadget lineups work from this location?
- What angles, counters, and failure points should I be aware of?

The focus is on operators whose utility interacts predictably with map geometry.

## The Problem

Useful Siege tactics are scattered across:

- YouTube videos
- Twitch and professional match VODs
- TikTok and other short-form videos
- Reddit posts
- Community Discord servers
- Personal strategy documents

Finding the correct tip during operator selection is slow. Content may also be outdated, incorrectly labeled, poorly explained, or dependent on an older map or operator version.

Watching a ten-minute video to find one placement is not practical when a player only has a short time before the round begins.

## Proposed Solution

The application provides a fast lookup flow:

1. Select a map.
2. Select a bomb site.
3. Select an operator.
4. Browse verified tactics for that exact combination.
5. Open a quick reference or a complete explanation.

A result may contain:

- An annotated overhead location
- A first-person “stand here” image
- The exact placement or aim point
- Step-by-step instructions
- The intended purpose
- Resulting lines of sight or destruction
- Required reinforcements, openings, or supporting utility
- Positions to hold after completing the setup
- Dangerous angles and common counters
- A fallback if the setup is destroyed or countered
- A short verification clip
- The game version and last verification date
- Attribution to the original source where applicable

## Example: Mira

For Mira on a selected bomb site, the application could show:

- Default, safe, aggressive, and coordinated Black Mirror placements
- Which wall panel should be reinforced
- Which direction the mirror should face
- Walls that should remain soft
- Supporting rotations, headholes, or footholes
- The lines of sight created by the placement
- Where Mira should hold and where she can retreat
- Vertical, window, doorway, and rappel threats
- Current counters and possible responses
- Related C4 lineups when available in the current loadout
- Alternative placements using Mira if the primary setup is unavailable

## Operators in Scope

The project does not need to support every operator.

An operator is a good fit when their useful actions can be:

- Anchored to a map, room, surface, or bomb site
- Planned before an enemy position is known
- Reproduced in an empty custom game
- Explained using exact visual instructions
- Independently tested and verified

Potential categories include:

### Defensive Setup

- Mira placements
- Kaid Electroclaw placements
- Mute jammer coverage
- Bandit battery positions
- Castle barricade setups
- Azami barrier placements
- Aruni gate placements
- Deployable shield positions
- Site cameras and observation utility
- Reinforcements, rotations, headholes, and footholes

### Attacking Setup

- Fuze Cluster Charge positions
- Ram deployment paths
- Zero camera locations
- Thermite, Hibana, and Ace breach locations
- Vertical destruction routes
- Drone preplacements
- Flank-watch placements
- Default plant positions
- Post-plant positions
- Grenade, projectile, and utility lineups

## Operators Out of Scope

Operators whose effectiveness mainly depends on unpredictable live information may not receive dedicated guides.

Examples include operators primarily centered around:

- Finding a specific enemy
- Reacting to the enemy team composition
- Taking gunfights
- Interpreting live intel
- Improvised ability use without a repeatable map location

The project should never create filler content merely to claim complete operator coverage.

If no useful, verified tactic exists for an operator on a site, the application should say so.

## Tip Types

Tactics can be organized by purpose:

- Gadget placement
- Camera placement
- Throwable lineup
- Vertical destruction
- Hard breach
- Wall or hatch denial
- Site construction
- Utility clearing
- Plant execution
- Plant denial
- Post-plant
- Sightline
- Holding position
- Retreat route
- Counter and fallback

## Potential Threats and Operator Synergies

Each tactic should identify the most likely threats to the selected operator’s setup.

Directly beneath those threats, a **Plays Well With** section may recommend supporting operators that teammates can bring to protect or strengthen the setup.

These are supporting recommendations only. The application does not need to show placements or complete guides for the supporting operators.

### Example: Mira

#### Potential Threats

- Hard-breach utility destroying the reinforced wall
- Projectiles or explosives clearing the position
- Vertical pressure above or below the mirror
- Attackers reaching the opposite side of the wall
- The mirror canister being exposed
- The Mira player losing a safe retreat route

#### Plays Well With

- **Kaid or Bandit — Wall denial**  
  Helps prevent attackers from breaching the wall holding the Black Mirror.

- **Wamai or Jäger — Projectile protection**  
  Helps intercept projectiles intended to clear utility or force the Mira player away from the position.

- **Mute — Disruption and drone denial**  
  Can make it harder for attackers to gather information or use compatible electronic utility near the setup.

Each recommendation should be connected to a specific threat rather than being presented as a generic team composition.

### Synergy Information

A synergy entry should contain:

- Supporting operator
- Support role
- Threat addressed
- One-sentence explanation
- Importance level
- Current patch verification

Suggested importance levels:

- **Required:** The tactic does not work as intended without this support.
- **Strong:** The support meaningfully improves the tactic’s reliability.
- **Optional:** Helpful, but the tactic remains functional without it.

### Tactic-Specific Recommendations

Synergies should be attached to the individual tactic, not only to the selected operator.

For example, one Mira placement may be especially vulnerable to hard breach and strongly benefit from Kaid or Bandit. Another may be protected from the opposite side but exposed to projectiles, making Wamai or Jäger more relevant.

The application should therefore present:

`Selected tactic → Potential threats → Plays Well With`

It should not assume that every placement for an operator has the same weaknesses or ideal supporting lineup.

### Recommendation Rules

Supporting recommendations must:

- Explain exactly what the supporting operator contributes
- Address a documented threat or dependency
- Reflect the current game version
- Account for unavailable or banned operators
- Avoid presenting any synergy as a guaranteed counter
- Avoid adding an operator merely because they are commonly selected
- Offer role-based alternatives when multiple operators provide similar support

The purpose of this section is to give the player a short, useful request they can communicate to teammates, such as:

> “This Mira setup is vulnerable to the wall being opened. Kaid or Bandit would help protect it.”

or:

> “This position can be cleared with projectiles. Wamai or Jäger would make it safer.”

## Quick View and Practice View

### Quick View

Designed for use during operator selection:

- One primary image
- A short purpose statement
- Two to four instructions
- Major danger or counter
- Patch verification badge

### Practice View

Designed for learning in a custom game:

- Full walkthrough
- Multiple visual references
- Exact stance and aim point
- Supporting setup requirements
- Explanation of why the tactic works
- Counters and failure conditions
- Repetition checklist
- Verification footage
- Original source and attribution

## Content Discovery

Potential tactics may be discovered through:

- Official R6 Esports VODs
- Professional player footage
- Creator videos
- Twitch clips
- Community posts
- Direct creator submissions
- User-submitted links
- Original testing and experimentation

Social popularity, view count, or professional usage does not automatically prove that a tactic is correct or generally useful.

A tactic observed in professional play should be labeled as an observation, not as “pro-approved.” Professional setups may rely on a particular team composition or coordinated strategy.

## Verification Process

Every public recommendation should pass a structured review process:

1. **Discovered**  
   A source or community member identifies a possible tactic.

2. **Triaged**  
   A curator confirms that it matches the project’s operator and placement scope.

3. **Reproduced**  
   A curator recreates the tactic on the current live game version.

4. **Documented**  
   Original instructions, screenshots, diagrams, and verification footage are created.

5. **Independently tested**  
   A second reviewer follows only the written instructions and attempts to reproduce the result.

6. **Published**  
   The tactic is added to the searchable library with its version and evidence.

7. **Reverification required**  
   Relevant map, operator, gadget, or physics changes automatically mark the tactic for review.

Suggested content lifecycle:

`Discovered → Testing → Verified → Published → Needs Retest → Retired`

## Source and Rights Handling

The project should preserve provenance without copying content unnecessarily.

For each discovered tactic, the database may record:

- Source platform
- Original URL
- Creator or team
- Video or post identifier
- Relevant timestamp
- Date discovered
- Permission or licensing status
- Curator notes

The public guide should use original screenshots, diagrams, descriptions, and verification footage whenever possible.

External videos should be linked or embedded through supported platform tools rather than downloaded and rehosted. Attribution does not replace permission.

## Versioning

Siege is continuously updated. Map geometry, bomb sites, gadget behavior, operator loadouts, and interactions can all change.

Every tactic should therefore record:

- Season or game build
- Map version
- Operator version
- Required loadout
- Platform tested
- Verification date
- Reviewer
- Relevant patch dependencies

Published tactics should never be silently overwritten. Changes should create a new revision while preserving the previous record.

## Proposed MVP

The first version should remain intentionally small:

- Bomb mode only
- One current map
- Every relevant bomb site on that map
- Four placement-focused operators:
  - Mira
  - Kaid
  - Fuze
  - Ram
- Two to four useful tactics per supported operator and site
- Quick and detailed views
- Search and filtering
- Patch and verification labels
- Source attribution
- “Outdated or incorrect” reporting
- Mobile-friendly web interface
- No account required for browsing

The MVP should prioritize correctness over content volume.

## Future Features

Possible later additions include:

- Additional placement-focused operators
- Additional maps
- Saved personal playbooks
- Solo, duo, and coordinated-team variants
- Beginner and advanced difficulty labels
- Interactive floor diagrams
- Community submissions
- Reviewer and contributor profiles
- Creator-curated collections
- Practice checklists
- Patch-impact dashboards
- Shareable tactic links
- Offline reference packs
- Team-specific private collections

## Non-Goals

The project is not intended to:

- Recommend which operator a player should select
- Generate unverified tactics using AI
- Support every operator
- Guarantee that a tactic will win a round
- Copy or rehost creator content without permission
- Read game memory or network traffic
- Provide live enemy information
- Function as a cheat, exploit database, or unauthorized game overlay

## Quality Principles

- No fabricated placements or results
- No “best setup” claims without evidence
- Every tactic must state its purpose
- Every conditional tactic must state its prerequisites
- Professional usage is evidence of use, not proof of universal effectiveness
- Independent reproduction matters more than popularity
- Outdated content should be hidden or clearly marked
- Fewer trustworthy tactics are better than a large unreliable library

## Success Criteria

The idea is successful if players can:

- Find a relevant tactic faster than searching through videos
- Reproduce it without assistance from its author
- Understand why it works
- Recognize its dangers and counters
- Trust that it was tested on the current game version
- Return to the application across multiple play sessions

## Disclaimer

This is an independent, unofficial fan project. It is not affiliated with, endorsed by, sponsored by, or licensed by Ubisoft.

Rainbow Six, Rainbow Six Siege, operator names, maps, artwork, and related trademarks are the property of Ubisoft and their respective rights holders.

Any public or commercial release must comply with Ubisoft’s terms, applicable platform policies, creator rights, and copyright law.