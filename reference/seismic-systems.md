# Seismic Structural Systems for Tall RC Buildings

This file provides the researcher's reference on lateral system options for tall reinforced concrete buildings. For each system, it covers the structural logic, the conditions under which it is appropriate, the key performance questions, and the sources that inform decision-making.

This is not a design specification. It is a decision-support framework.

---

## Core Wall System

**Structural logic:**
A central reinforced concrete core — typically surrounding elevator shafts, stairs, and services — acts as the primary lateral force-resisting element. The core behaves as a vertical cantilever. Gravity columns at the perimeter carry vertical load but contribute minimally to lateral resistance unless explicitly designed to do so.

**When appropriate:**
- Regular plan geometry with sufficient core dimensions to provide required stiffness and strength
- Buildings where architectural programming concentrates services centrally
- Height range approximately 20–60 stories, depending on seismic demand and core geometry
- DCM or DCH target achievable with coupling beam design

**Key performance questions:**
- What is the core wall aspect ratio (height-to-width)? Slender cores in high seismicity may be governed by overturning and foundation demand rather than shear.
- Are coupling beams included? Coupled core walls significantly outperform uncoupled walls in ductility and energy dissipation. Coupling beam design is critical — diagonally reinforced coupling beams per EC8/ACI 318 are required for DCH.
- What is the expected failure mechanism? Core wall systems should be designed for a ductile flexural mechanism at the base, not a shear-dominated response.
- Has the core-to-floor connection been designed for diaphragm shear transfer?

**Sources:**
EC8 Part 1 Section 5 (RC structures), fib Bulletin 39, PEER TBI Guidelines, LATBSDC

---

## Wall-Frame Dual System

**Structural logic:**
Shear walls (or a core) combined with moment-resisting frames. Both systems contribute to lateral resistance. EC8 defines a dual system as one where frames resist at least 25% of the total seismic base shear. This shared resistance provides redundancy and typically improves regularity.

**When appropriate:**
- Buildings where perimeter frame geometry is architecturally compatible with seismic frame behavior
- Situations where core geometry alone is insufficient for required stiffness
- Where plan irregularity from core-only system would be problematic
- Heights where wall-alone system would produce excessive drift without perimeter contribution

**Key performance questions:**
- Is the 25% frame contribution (EC8 dual system criterion) actually being achieved in the structural model, or is it assumed?
- Are frame-wall interaction forces being captured? At intermediate floors, the wall and frame interact — the wall tends to restrain the frame at lower levels and be restrained by the frame at upper levels. These interaction forces must be designed for.
- Has the frame been designed for ductile behavior — strong column-weak beam mechanism — or is the frame being treated as gravity-only with lateral participation assumed?

**Sources:**
EC8 Part 1 Section 5.2.2 (structural types and behavior factors), SEAOC Bluebook, LATBSDC

---

## Outrigger System

**Structural logic:**
One or more stiff outrigger trusses or walls connect the central core to perimeter mega-columns or walls at discrete levels. This connection transfers lateral loads from the core into axial forces in the perimeter columns, significantly reducing core overturning moment and increasing overall building stiffness.

**When appropriate:**
- Buildings above approximately 50–60 stories where core-alone stiffness is insufficient for drift control
- Where large perimeter columns can be architecturally accommodated
- Where mechanical or plant floors provide a structural opportunity for outrigger placement
- Where very high lateral stiffness is required to control wind-induced motion (occupant comfort) alongside seismic performance

**Key performance questions:**
- What is the outrigger level location? Optimum location for stiffness efficiency is typically between 40–70% of building height, but structural and architectural constraints usually govern.
- How many outrigger levels are planned? One vs. two vs. three levels affects the stiffness profile and the redundancy of the system.
- How is the outrigger-core connection detailed for seismic loading? Under seismic demand, the outrigger connection transfers significant shear and moment — this is a critical connection.
- Has differential axial shortening between core and perimeter columns been addressed? In tall buildings, differential shortening over the construction period can induce significant forces in outrigger connections before the building is even loaded.
- What is the seismic behavior factor for an outrigger-enhanced system? EC8 does not explicitly categorize outrigger systems — the behavior factor must be justified based on the overall system behavior and precedent.

**Sources:**
CTBUH Journal (outrigger system case studies), PEER TBI Guidelines, LATBSDC, Taranath (Structural Analysis and Design of Tall Buildings)

---

## Flat Slab Systems in Seismic Regions

**Structural logic:**
Flat slabs span directly from column to column without beams. Lateral resistance is provided by a separate core or shear wall system. The flat slab is nominally assumed to act as a diaphragm and gravity system but not as part of the lateral force-resisting system.

**When appropriate:**
- Residential or hotel buildings where clear ceiling height is a premium requirement
- Lower-to-mid-rise buildings (typically below 30–35 stories) in moderate seismicity
- Where core wall lateral resistance is sufficient without frame contribution

**Critical warnings — assumptions that must be verified:**

*Punching shear under seismic drift:*
Flat slab connections to columns are vulnerable under the combined demands of gravity loads and seismic-induced lateral drift. EC8 Section 5.11 and ACI 318-19 Section 18.14 address this, but detailing requirements are demanding. fib Bulletin 68 provides detailed research on post-punching behavior. This must be explicitly designed and checked — it cannot be assumed acceptable.

*Diaphragm behavior:*
The flat slab is assumed to transfer in-plane forces to the core. At the slab-core connection, in-plane shear demand under seismic loading can be significant. This must be analyzed and designed, not assumed.

*Drift amplification:*
Without perimeter beams, the lateral stiffness of the floor system is reduced. Under seismic loading, slab-column frames can experience significant inelastic drift. EC8 Section 5.11.1.3 requires that in DCM and DCH buildings, the rotation demands at slab-column connections be verified.

*Ductility class limitation:*
Flat slab frames are generally not considered suitable for DCH due to the difficulty of providing adequate ductility at slab-column connections. DCM may be appropriate in moderate seismicity with careful detailing.

**Sources:**
EC8 Part 1 Section 5.11, fib Bulletin 68, ACI 318-19 Section 18.14, PEER reports on slab-column connection performance

---

## Tube Systems

**Structural logic:**
The building perimeter acts as a hollow tube — closely spaced perimeter columns connected by deep spandrel beams. The entire perimeter frame resists lateral load through frame action. Particularly efficient for very tall buildings where perimeter framing can be tightly controlled.

**When appropriate:**
- Buildings above 60–80 stories where maximum efficiency of material is required
- Where architectural expression of the structural tube is compatible with the building program
- Primarily used in steel or composite construction; less common in pure RC

**Key performance questions:**
- Shear lag in tube systems: under lateral loading, axial forces in the tube columns are not uniform — corner columns carry more than mid-face columns. This shear lag effect must be quantified in analysis.
- Framed tube vs. bundled tube vs. trussed tube: each variant has different stiffness and constructability characteristics.

**Sources:**
CTBUH, Taranath, PEER TBI Guidelines

---

## System Selection Decision Framework

When evaluating lateral system options, the researcher should assess each system against:

| Criterion | Questions |
|-----------|-----------|
| Seismic demand | Is the system capable of achieving the required behavior factor and ductility for the site demand? |
| Plan geometry | Does the architectural plan support the structural logic of the system? |
| Height and aspect ratio | Is the system appropriate for the building's height and slenderness? |
| Regularity | Does the system produce a regular or irregular stiffness and mass distribution? |
| Detailing achievability | Can the required ductile detailing be reliably executed on this project? |
| Precedent | Are there comparable projects in similar seismic environments? |
| Code compliance | Does the system fall within EC8 prescriptive scope, or does it require PBD? |
