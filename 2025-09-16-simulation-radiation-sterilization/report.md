# Scientific Exchange on Modeling and Simulation for Radiation Sterilization

*From exchange to engagement: insights to move our collaboration forward.*

**September 16–17, 2025 | NIST, Gaithersburg**

## Table of Contents <!-- omit in toc -->

- [1. Executive Snapshot](#1-executive-snapshot)
- [2. Purpose and Context](#2-purpose-and-context)
  - [2.1. Why This Exchange Mattered](#21-why-this-exchange-mattered)
  - [2.2. Intended Outcomes](#22-intended-outcomes)
  - [2.3. The Stakes](#23-the-stakes)
- [3. Highlights and Emerging Themes](#3-highlights-and-emerging-themes)
  - [3.1. Theme 1: Establishing Trust Through Rigorous Validation](#31-theme-1-establishing-trust-through-rigorous-validation)
    - [3.1.1. The Situation](#311-the-situation)
    - [3.1.2. What Emerged](#312-what-emerged)
    - [3.1.3. Why it matters](#313-why-it-matters)
  - [3.2. Theme 2: High-Value Applications to Demonstrate Worth](#32-theme-2-high-value-applications-to-demonstrate-worth)
    - [3.2.1. The Situation](#321-the-situation)
    - [3.2.2. What Emerged](#322-what-emerged)
    - [3.2.3. Why it matters](#323-why-it-matters)
  - [3.3. Theme 3: Building the Missing Infrastructure](#33-theme-3-building-the-missing-infrastructure)
    - [3.3.1. The Situation](#331-the-situation)
    - [3.3.2. What Emerged](#332-what-emerged)
    - [3.3.3. Why it matters](#333-why-it-matters)
- [4. Knowledge Gaps and Open Questions](#4-knowledge-gaps-and-open-questions)
- [5. Key Insights and Takeaways](#5-key-insights-and-takeaways)
- [6. Opportunities and Next Steps](#6-opportunities-and-next-steps)
- [7. Disclosure on the use of Generative AI](#7-disclosure-on-the-use-of-generative-ai)
- [8. Annex](#8-annex)

## 1. Executive Snapshot

This exchange brought together 47 participants from 30 organizations — spanning academia, government, manufacturers, radiation processing facilities, and regulatory bodies — to address one fundamental question: *How can ionizing radiation simulation earn the same credibility in radiation sterilization that it has achieved in other fields?* Over two days, the group identified three converging priorities: (1) establishing validation frameworks that quantify uncertainty and define model limits; (2) demonstrating practical use cases where simulation can reduce or replace physical dosimetry without compromising safety; and (3) building regulatory confidence through standardized reference materials and credentialing processes. Participants from radiation oncology described how their field navigated similar challenges decades ago, offering a roadmap that sterilization could adapt. Most importantly, the exchange moved beyond identifying problems to outlining specific actions — forming working groups, conducting round-robin studies, and developing guidance documents — that could shift modeling from an underutilized tool to a recognized standard. This report captures what emerged from those discussions, where disagreements surfaced, and how to maintain momentum toward a future where simulation is as trusted for ensuring sterile products as it already is for treating cancer patients.

## 2. Purpose and Context

### 2.1. Why This Exchange Mattered

This scientific exchange convened leading researchers, industry practitioners, and regulatory representatives to strengthen international collaboration on modeling and simulation methods for radiation sterilization. The context is critical: while radiation oncology has relied on computational models to plan treatments for cancer patients for decades, the sterilization industry — charged with ensuring medical devices are safe before they reach those same patients — remains largely dependent on physical dosimetry. This gap is not academic. As medical devices grow more complex in geometry and materials, and as supply chains demand greater efficiency without compromising safety, the traditional approach of placing hundreds of dosimeters throughout validation runs becomes increasingly costly, time-intensive, and sometimes inadequate for capturing dose distributions in intricate geometries. The exchange emerged from a recognition that closing this gap requires more than better software. It demands metrological standards for validation, clarity on uncertainty quantification, regulatory frameworks that reward rigor rather than resist innovation, and a community willing to learn from fields that have already made this transition successfully.

### 2.2. Intended Outcomes

`Lead`

- **Learn from radiation oncology’s playbook** by understanding how a parallel field successfully integrated computational modeling into clinical practice, then adapt those lessons to industrial sterilization contexts.

- **Establish a multi-year roadmap** with clear milestones for advancing modeling and simulation adoption in radiation sterilization: moving from concept to consensus on actionable priorities.

- **Define technical requirements** for verification, validation, and uncertainty quantification that the community could rally around as shared standards.

- **Build pathways to regulatory credibility** by identifying what evidence, documentation, and validation frameworks would give regulators confidence in simulation-based approaches.

- **Identify immediate next steps** beyond the meeting: reference phantoms, benchmark problems, working group structures, and pilot collaborations that could begin mobilizing resources and expertise.

### 2.3. The Stakes

The discussions revealed that different communities face distinct but interconnected stakes, all pointing toward the same conclusion: *the current state is holding everyone back.*

- **For medical device manufacturers:** Extensive physical dosimetry requirements translate directly into longer validation timelines and higher costs, slowing the introduction of innovative devices and constraining supply chain flexibility when product changes are sought or required.

- **For radiation processing facilities:** The inability to leverage validated simulation means forgoing efficiency gains and parametric release opportunities that could improve throughput and reduce routine dosimetry burden without compromising sterility assurance.

- **For regulators:** The tension between protecting patient safety and enabling innovation is acute. Overly conservative approaches to modeling can inadvertently stifle the very innovations that improve healthcare outcomes, yet accepting simulation without rigorous validation frameworks is untenable.

- **For the measurement science community:** The exchange positioned them as uniquely capable neutral conveners with the technical credibility to establish reference standards, the institutional standing to engage regulators, on their mission to enable innovation through rigorous metrology.

- **The ultimate stake:** Whether the sterilization field will remain constrained by validation approaches developed in an earlier era, or build the measurement infrastructure needed to meet the demands of increasingly complex medical devices and global supply chains.

## 3. Highlights and Emerging Themes

If this conversation feels familiar, it should. For over a decade, discussions about modeling and simulation in radiation sterilization have followed a predictable arc: recognition that simulation could transform the field, followed by concerns about trust, followed by what is needed to build confidence — without coalescing into coordinated action.

What made this exchange different was the will to break that cycle. Rather than rehearsing why simulations are not yet trusted, participants used that shared recognition as a starting point for something more productive: identifying *exactly* where the bottlenecks are, *specifically* where early wins could demonstrate value, and *concretely* what infrastructure needs to exist. The themes that emerged are not new problems, they are persistent challenges. This community has now decided to tackle them systematically rather than revisit indefinitely. What follows captures not just what was discussed, but where the group found traction for actual progress.

### 3.1. Theme 1: Establishing Trust Through Rigorous Validation

#### 3.1.1. The Situation

The sterilization community has access to mature simulation tools, yet they remain largely unused for regulatory submissions or routine operations. The gap is not technical capability, it is *credibility.*

#### 3.1.2. What Emerged

- **Radiation oncology offered a blueprint.** Participants from that field described how they built trust through systematic commissioning protocols, quality assurance frameworks, professional society guidelines (like AAPM documents), and mandatory training requirements for anyone using treatment planning software. The message was clear: credibility came not from better algorithms or software toolkits, but from institutional structures that ensured consistent, verified application.

- **Verification, validation, and uncertainty quantification are non-negotiable.** Multiple breakout sessions converged on the same conclusion: without rigorous frameworks for quantifying what models can and cannot predict reliably, adoption will stall. Participants identified four specific risks that must be addressed systematically:

  - *Sensitivity to product positioning:* Predictions degrade when exact placement within the radiation field varies. *Mitigation:* Conduct a sensitivity analysis on all the degrees of freedom, recommend clear restraints or limits on positioning variability

  - *Degradation due to unmonitored system parameters:* Accuracy suffers if beam current, temperature, or other process variables drif, undetected. *Mitigation:* Conduct a sensitivity analysis on all critical, observable parameters, develop periodic recommendations for resetting the system or recalibrating the model input.

  - *Fundamental accuracy limitations:* The model’s physics or parameterization may not capture all relevant phenomena reliably. *Mitigation:* Assemble a sufficient amount of ground truth data. This includes data collected from the actual process and, crucially, data derived from independently engineered phantoms that provide clear, unambiguous validation points.

  - *Users applying model to out-of-scope scenarios:* Extending predictions to doses, geometries, or materials outside validated conditions. *Mitigation:* Conduct a thorough investigation of the limits of the model, publish clear guidelines on the model’s applicability.

- **The credibility problem is as much cultural as technical.** Several participants noted that even when models perform well, regulators and industry practitioners remain skeptical because there are no agreed-upon standards for what constitutes adequate validation. We keep asking *"is the model good enough?"* without first agreeing on what *"good enough"* means in practice.

#### 3.1.3. Why it matters

Without standardized validation, modeling cannot transition from research to practice. The identified risks — positioning uncertainty, parameter drift, measurement limitations, and operator proficiency — are universal in dosimetry, whether computational or physical. Simulation’s key advantage is enabling rapid sensitivity studies to quantify and mitigate these universal risks in ways that would be experimentally prohibitive.

### 3.2. Theme 2: High-Value Applications to Demonstrate Worth

#### 3.2.1. The Situation

Rather than positioning simulation as a disruptive replacement for physical dosimetry, participants identified specific, near-term applications where modeling could deliver immediate value while building the evidence base for broader adoption.

#### 3.2.2. What Emerged

- **Strategic dosimeter placement tops the list.** Using simulation to optimize where dosimeters should be positioned during validation runs addresses a current pain point without requiring anyone to trust the model for absolute dose predictions. This “low-risk, high-value” application could generate confidence while maintaining existing safety margins.

- **Product change management as a compelling use case.** When manufacturers modify device geometry or materials, current practice requires extensive *revalidation*. Simulation could demonstrate functional equivalence between the old and new configurations, potentially reducing the dosimetry burden while maintaining sterility assurance. Several industry participants cited this as where they would most readily adopt validated modeling approaches.

- **Parametric release represents the long-term vision.** Multiple participants described scenarios where validated models, combined with real-time monitoring of process parameters, could enable product release based on process control rather than routine dosimetry. X-ray sterilization was identified as a particularly promising starting point, given its tighter process control compared to gamma or electron beam.

#### 3.2.3. Why it matters

By complementing rather than replacing existing practices, the field can build evidence incrementally of simulation’s accuracy and value relative to physical dosimetry. This gradual approach gains regulatory acceptance without requiring immediate wholesale change.

### 3.3. Theme 3: Building the Missing Infrastructure

#### 3.3.1. The Situation

Even participants enthusiastic about modeling acknowledged that key infrastructure components — reference materials, standardized test cases, and institutional mechanisms — exist but remain fragmented.

#### 3.3.2. What Emerged

#### 3.3.3. Why it matters

## 4. Knowledge Gaps and Open Questions

## 5. Key Insights and Takeaways

## 6. Opportunities and Next Steps

## 7. Disclosure on the use of Generative AI

Generative AI was used to structure and refine this report, drawing exclusively from participant notes and materials. All substantive content has been verified by the authors, who assume full accountability for the accuracy and integrity of what appears in this document.

## 8. Annex
