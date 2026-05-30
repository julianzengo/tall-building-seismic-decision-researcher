# Key Concepts

A working reference for the core concepts that recur in tall building seismic research. These are the terms and ideas the researcher must understand precisely to investigate effectively.

---

## Behavior Factor (q)

The behavior factor is the ratio between the elastic seismic force demand and the reduced design force. It accounts for ductility (the ability to deform inelastically without collapse), overstrength (the reserve capacity beyond first yield), and energy dissipation.

**In EC8:** q values range from 1.5 (DCL) to approximately 5.5 (DCH wall systems). Higher q reduces design forces but requires more demanding ductile detailing.

**Critical point:** The behavior factor is only valid if the ductility capacity it assumes is actually achievable — through appropriate structural system, detailing, and construction quality. An assumed q that is not backed by achievable ductility is an unsafe assumption.

---

## Ductility

The ability of a structural element or system to undergo large inelastic deformation without significant loss of strength. In seismic design, ductility allows the structure to absorb energy during strong shaking rather than failing suddenly.

**Global ductility:** The overall deformation capacity of the building before collapse.
**Local ductility:** The deformation capacity of individual elements — typically the critical plastic hinge regions at the base of walls and ends of coupling beams and frame members.

**EC8 approach:** Ductility is achieved through confinement of concrete in critical regions, careful detailing of shear reinforcement, control of lap splice locations, and capacity design of non-ductile elements.

---

## Capacity Design

A design philosophy in which the structure is designed so that inelastic deformation (plastic hinging) occurs only in designated ductile zones, while all other elements are designed to remain elastic by having sufficient strength to resist the forces generated when the ductile zones reach their maximum probable capacity.

**In a core wall building:** The core wall base is designed as the ductile zone (plastic hinge). All elements above — coupling beams, foundation, connections — are designed for the forces that develop when the wall base reaches its overstrength capacity.

**Researcher flag:** Capacity design must be implemented consistently throughout the structural system. A chain is only as strong as its weakest link — if a non-ductile element is not designed for capacity design forces, it may fail before the intended ductile mechanism develops.

---

## Regularity — Plan and Elevation

**Plan regularity (EC8 Section 4.2.3.2):**
A building is regular in plan if it has compact geometry, approximately symmetric stiffness and mass distribution, and limited eccentricity between center of mass and center of stiffness (≤30% of torsional radius). Regular buildings may use simplified analysis methods.

**Elevation regularity (EC8 Section 4.2.3.3):**
A building is regular in elevation if lateral stiffness and mass are approximately uniform with height and there are no significant discontinuities (soft stories, mass concentrations, setbacks exceeding code limits).

**Why it matters:** Irregular buildings must use more sophisticated analysis methods, may have reduced behavior factors, and require explicit checks for torsional response and story mechanism formation.

---

## Torsional Response

Occurs when the center of stiffness and center of mass of a building are not coincident. Under seismic loading, the building twists as well as translates, causing amplified demands on elements distant from the stiffness center.

**EC8 treatment:** Plan regularity criteria limit eccentricity. For irregular buildings, dynamic analysis captures torsional modes. Accidental torsion must also be accounted for by offsetting the mass by 5% of the floor dimension.

**Tall building sensitivity:** In tall buildings, torsional irregularity can be particularly damaging because torsional deformation amplifies story drift at perimeter elements through the full building height.

---

## Performance-Based Earthquake Engineering (PBEE)

A design philosophy that explicitly links structural performance to seismic hazard levels. Rather than prescribing detailing rules and behavior factors (as EC8 does), PBEE quantifies the expected structural response at defined hazard levels and checks that response against explicit performance targets.

**PEER PBEE framework:**
- Hazard analysis: probability of exceeding ground motion intensity levels
- Structural analysis: nonlinear response at those intensity levels
- Damage analysis: expected damage to structural and non-structural components
- Loss analysis: expected repair costs, downtime, casualties

**For tall buildings:** PBEE is the appropriate framework when prescriptive code approaches are insufficient — typically for buildings that exceed height limits, have irregular configurations, or use structural systems not explicitly addressed in the code.

---

## Site-Specific Seismic Hazard Analysis (PSHA)

Probabilistic Seismic Hazard Analysis quantifies the probability of exceeding various ground motion intensity levels at a specific site, accounting for all relevant seismic sources, their activity rates, and ground motion propagation.

**When required for tall buildings:**
- Buildings exceeding code height limits
- Sites with unusual ground conditions
- Buildings with high importance factors
- When EC8 standard spectra are considered insufficient for the site's tectonic environment

**Output:** A site-specific hazard curve and (for structural analysis) a Uniform Hazard Spectrum (UHS) or Conditional Mean Spectrum (CMS) at specified return periods.

---

## Soil-Structure Interaction (SSI)

The mutual influence between a structure's dynamic response and the behavior of the supporting soil. In stiff buildings on soft soil, the soil modifies the input motion (kinematic interaction) and the building's inertia loads deform the soil (inertial interaction).

**EC8 Part 5:** Requires SSI to be considered when it may adversely affect the structure — particularly for stiff structures on soft soil, piled foundations in liquefiable ground, and buildings adjacent to slopes.

**Tall building note:** SSI can either increase or decrease seismic demand depending on the building-soil frequency relationship. It cannot be assumed to be beneficial without analysis.

---

## Liquefaction

The process by which saturated, loosely packed cohesionless soils lose strength and behave like a liquid under cyclic loading (seismic shaking). Liquefaction can cause foundation settlement, lateral spreading, loss of pile lateral capacity, and floating of buried structures.

**EC8 Part 5 assessment:** Required for loose saturated sands and silts below the water table in seismic zones. EC8 Section 4.1.3 defines conditions under which liquefaction potential may be neglected.

**Researcher flag:** Liquefaction assessment must be based on site-specific geotechnical investigation — CPT and SPT testing with appropriate corrections. Map-based or assumed assessments are insufficient for a tall building foundation decision.

---

## Nonlinear Analysis — Static and Dynamic

**Nonlinear Static Analysis (Pushover):**
The structure is subjected to monotonically increasing lateral load until failure. Captures the inelastic force-deformation relationship and identifies plastic hinge formation sequence. EC8 Annex B provides a nonlinear static procedure. Useful for identifying weak stories and checking global mechanism.

**Nonlinear Dynamic Analysis (Time-History):**
The structure is subjected to a suite of ground motion records. Captures the dynamic inelastic response including duration effects, higher mode contributions, and record-to-record variability. Required by PEER TBI and LATBSDC for tall buildings. Considered by EC8 as an alternative to response spectrum analysis.

**For tall buildings:** Nonlinear dynamic analysis is the standard of practice for performance-based design. The number of records, selection and scaling methodology, and acceptance criteria (mean vs. maximum of suite) are defined by PEER TBI and LATBSDC.

---

## Inter-Story Drift and Global Drift

**Inter-story drift:** The relative horizontal displacement between two adjacent floors, usually expressed as a ratio of the story height (drift ratio). It is one of the most important response quantities in tall building seismic design because it governs damage to structural and non-structural elements.

**Global drift:** The total lateral displacement at the top of the building relative to its base, expressed as a ratio of total height.

**EC8 treatment:** The damage limitation requirement (EC8 Section 4.4.3.2) limits inter-story drift under the frequent (serviceability) seismic action — typically 0.5% to 1.0% of story height depending on the type of non-structural elements and how they are attached to the structure.

**Why it dominates tall building design:** For tall, slender buildings, drift — not strength — frequently governs the lateral system. A building can have ample strength yet fail serviceability and damage-limitation checks on drift. The lateral system is often sized by drift control, which is why stiffness (not just capacity) drives system selection. This is also where wind and seismic compete: in moderate seismicity, wind drift may govern.

---

## P-Delta Effects (Second-Order Geometric Effects)

The additional forces and displacements that arise when gravity loads act on a laterally displaced structure. As the building sways, the vertical loads acting through the lateral displacement create additional overturning demand, which increases displacement further — a potentially destabilizing feedback loop.

**EC8 treatment:** EC8 Section 4.4.2.2 defines the inter-story drift sensitivity coefficient θ (theta). When θ ≤ 0.10, P-delta may be ignored. When 0.10 < θ ≤ 0.20, P-delta effects may be approximated by amplifying lateral effects by 1/(1−θ). When 0.20 < θ ≤ 0.30, a more rigorous second-order analysis is required. θ must not exceed 0.30.

**Tall building significance:** Slender tall buildings with significant drift are particularly sensitive to P-delta. The coefficient θ should be checked at every story, not just globally — it is often largest at intermediate levels, not the base. Ignoring P-delta in a slender tower is a common and consequential assumption that must be challenged.

---

## Diaphragm Behavior — Rigid, Flexible, Semi-Rigid

The floor diaphragm transfers in-plane seismic forces from the floor mass to the vertical lateral-resisting elements (cores, walls, frames) and ties the structure together so it responds as a unit.

**Rigid diaphragm:** Assumed to undergo no in-plane deformation; distributes forces to vertical elements in proportion to their relative stiffness. This is the standard assumption for most concrete floor systems and the basis for most analysis models.

**Flexible diaphragm:** Deforms significantly in-plane; distributes forces by tributary area rather than stiffness. More common in steel deck or timber systems.

**Semi-rigid diaphragm:** Intermediate behavior requiring explicit modeling of in-plane stiffness.

**Tall building flag:** The rigid diaphragm assumption is frequently challenged in real tall buildings by large floor openings (atria, mechanical shafts), long narrow floor plates, transfer levels, and slab-core connection details. Where the diaphragm cannot be confidently assumed rigid — particularly at transfer floors and podium levels — its in-plane behavior and force-transfer capacity must be explicitly analyzed and designed. This is especially critical for flat slab systems, where the slab is both the diaphragm and the gravity system.

---

## Coupling Beams

Short, deep beams connecting adjacent RC walls (or core wall segments) at each floor level. When designed correctly, coupling beams act as ductile energy-dissipating fuses — yielding in flexure or shear before the walls reach their capacity, thereby reducing wall demand and providing energy dissipation.

**DCH detailing:** EC8 and ACI 318 require diagonally reinforced coupling beams for high ductility applications (typically span-to-depth ratio below 2.0–2.5). The diagonal reinforcement must be properly confined to achieve the intended ductility.

**Researcher flag:** Coupling beam behavior is one of the most technically demanding aspects of core wall system design. The assumed level of coupling (and therefore the reduction in wall overturning moment) must be verified through analysis and achievable through detailing and construction. Assumed coupling that is not deliverable in practice is an unsafe assumption.
