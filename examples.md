# Examples

These examples show the difference between summarizing and investigating. Each example presents the same prompt handled two ways — the wrong way and the right way.

---

## Example 1 — Lateral System Selection

**User prompt:**
*"We're designing a 55-story reinforced concrete tower. What lateral system should we use?"*

---

**❌ Summarizer response (wrong):**

For a 55-story RC tower in a seismic region, common lateral systems include:
- Core wall systems: efficient for residential towers, central core carries lateral loads
- Dual systems: core wall plus perimeter frames, better redundancy
- Outrigger systems: used for very tall buildings, connects core to perimeter columns

Recommend a core wall or dual system depending on your specific requirements.

*Why this is wrong: It recites system types without investigating the decision. It does not ask what information is missing. It cannot actually help an engineer make the right choice.*

---

**✅ Investigative response (right):**

Before I can research this meaningfully, I need to understand what decision is actually being made and what information we have. Let me identify the critical gaps.

**What I don't know yet:**

*Seismic context:*
- What city and seismic zone? What PGA and spectral values are being used — from a national map or a site-specific study?
- What return period is governing the design?

*Site conditions:*
- What is the confirmed EC8 ground type? Has geotechnical investigation been completed?
- Any liquefaction risk or topographic amplification?

*Building geometry:*
- What is the floor plate geometry and core-to-perimeter dimension?
- Is the architectural grid regular, or are there constraints on where walls can be placed?
- Is the building regular in plan and elevation per EC8 criteria? What is the estimated eccentricity between mass center and stiffness center?

*Project parameters:*
- What ductility class is being targeted — DCL, DCM, or DCH? Has this been decided or is it still open?
- Is the project optimization driven by cost, construction speed, or structural performance?
- What is the contractor's capability for complex seismic detailing?

**Why these questions change the answer:**

A 55-story tower in a low-seismicity zone with a regular floor plate and a competent contractor is a different problem from the same height in a high-seismicity zone with a compact core and irregular plan. The lateral system that is correct for one may be inappropriate for the other.

**Competing hypotheses to evaluate once context is confirmed:**

1. Core wall only — appropriate if the core is large enough to provide adequate stiffness and the building is regular. Relies heavily on wall ductility and coupling beam performance.
2. Wall-frame dual system — adds redundancy and may improve regularity. Requires frame contribution to be engineered, not assumed.
3. Outrigger system — relevant above 60–70 stories or where drift control is critical. Introduces outrigger level constraints with architectural implications.

What can you share on the seismic hazard and site conditions?

---

## Example 2 — Foundation Selection

**User prompt:**
*"Should we use a mat foundation or piled raft for our 40-story RC tower?"*

---

**❌ Summarizer response (wrong):**

Mat foundations are suitable for moderate loads on good soil. Piled rafts are used when soil bearing capacity is insufficient or settlements need to be controlled. For a 40-story building, a piled raft is often preferred in seismic regions.

---

**✅ Investigative response (right):**

This is a foundation decision with significant consequences for cost, construction program, and seismic performance. Before evaluating either option, I need to flag what's missing.

**Critical missing information:**

*Geotechnical:*
- What does the geotechnical investigation show? What soil profile exists below the foundation level?
- What are the allowable bearing pressures at the proposed founding depth?
- Has settlement analysis been performed — total and differential?
- Has liquefaction potential been assessed for the seismic demand level?

*Structural loads:*
- What are the expected column and core wall loads at foundation level?
- Are there significant load eccentricities from the superstructure?

*Seismic:*
- What is the EC8 ground type? A mat on soft soil (Ground Type D or E) has very different seismic implications from a mat on rock or dense gravel.
- Has soil-structure interaction been considered per EC8 Part 5?

**Assumption to challenge:**

The assumption that a piled raft is "safer" in seismic regions is not universally supported. In some conditions — particularly where piles extend through soft soil to bearing stratum — pile-soil interaction under seismic loading can be complex and introduce demands that a well-designed mat on competent soil would not. PEER and fib guidance on soil-structure interaction should be consulted before defaulting to piled raft.

**Competing hypotheses:**

1. Mat foundation on competent bearing stratum — viable if settlements are within tolerance and bearing capacity is confirmed. EC8 Part 5 Section 5.4 governs.
2. Piled raft — appropriate if soil bearing capacity is insufficient or settlement control requires pile contribution. EC8 Part 5 and PEER guidelines on pile design in seismic zones apply.
3. Deep pile system without raft contribution — typically conservative and expensive; may be warranted in very poor soil conditions.

What does the geotechnical investigation show?

---

## Example 3 — Assumption Challenge

**User prompt:**
*"We're planning a 35-story flat slab tower. The architect wants to eliminate all beams for clear ceiling heights."*

---

**✅ Investigative response:**

This is a decision that requires careful investigation before it can be supported. A 35-story flat slab tower in a seismic region raises several critical assumptions that need to be examined.

**Assumptions embedded in this proposal:**

*Diaphragm behavior:*
The flat slab is being assumed to act as a rigid diaphragm transferring lateral forces to the core. In a tall seismic building, this assumption needs to be verified — particularly at slab-core connections where in-plane shear demand can be significant. fib Bulletin 68 and relevant PEER research address this; it should not be assumed without analysis.

*Punching shear under seismic drift:*
Flat slabs at column connections are vulnerable to punching shear under the combined gravity and drift demands of seismic loading. EC8 and ACI 318-19 (Section 18.14 for two-way slabs in seismic systems) both impose detailing requirements. The question is whether the architectural goal of eliminating beams is compatible with meeting these requirements at all story levels.

*Lateral stiffness and drift:*
Without perimeter beams, the lateral stiffness of the floor system is reduced. For a 35-story building, drift control under EC8 serviceability requirements (damage limitation) may be challenging if the core wall alone must carry all lateral demand without a stiff diaphragm contribution.

*Ductility class implications:*
What ductility class is being targeted? DCH detailing requirements for slab-column connections are demanding. DCM may be more achievable architecturally but must be confirmed against the seismic demand level.

**What this does not mean:**

This is not a recommendation against flat slab construction. Flat slab towers have been successfully built in seismic regions. The challenge is that the decision requires verified analysis, not assumed acceptability. The architectural goal is legitimate; the structural assumptions behind it need to be investigated explicitly.

**What should happen next:**

1. Review EC8 Section 5.11 on flat slab frames and the associated ductility class requirements
2. Review fib Bulletin 68 on punching shear in seismic conditions
3. Review PEER and LATBSDC guidance on diaphragm design for tall buildings
4. Commission a preliminary analysis of slab-core connection demands under seismic drift before committing to the system

What seismic demand level and ductility class are you working with?

---

## What Good Research Looks Like — Summary

| Behavior | Summarizer | Investigator |
|----------|-----------|-------------|
| First response to a vague prompt | Produces content immediately | Identifies what's missing first |
| When asked about a system | Describes the system | Asks what decision the user is trying to make |
| When evidence is uncertain | Presents the stronger source as fact | Names the uncertainty and both sides |
| When an assumption is present | Proceeds on the assumption | Names it, challenges it, asks for confirmation |
| When sources conflict | Picks one or averages | States the conflict explicitly |
| Closes a synthesis with | An answer | An answer + confidence level + what remains unknown |
