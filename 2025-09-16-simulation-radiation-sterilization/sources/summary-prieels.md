**September 16--17, 2025 \| NIST Gaithersburg Campus, Gaithersburg, Maryland**

D. Prieels, 24/09/25

This event was co-hosted by **NIST** and the **Council on Ionizing Radiation Measurements and Standards (CIRMS)**.

Event Page: <https://www.nist.gov/news-events/events/2025/09/scientific-exchange-modeling-and-simulation-radiation-sterilization>

**Technical Committee**

-   John Logar -- J&J

-   Cody Wilson -- IBA

-   Xun Jia -- John Hopkins

-   Ileana Pazos -- NIST

-   Spencer Mickum -- STERIS

-   Frederic Tessier -- NRC Canada (absent!)

-   Shaheen Dewji -- Georgia Institute of Technology

**Target Stakeholder Groups**

-   Healthcare Companies

-   Radiation Therapy Companies

-   Sterilization Companies

-   Regulatory Agencies

-   Notified Bodies

-   Academic Institutions

-   Industry Associations -- CIRMS, ASTM (E61), The Irradiation Panel, AAPM

# Context & Objective

*Despite the growing potential of mathematical modeling and simulation to transform industrial radiation sterilization, widespread adoption remains limited. This stems not from technical constraints, but from a lack of shared scientific frameworks, standardized verification methods, and clear quality assurance processes. As a result, modeling is often seen as supplementary rather than foundational, and industries continue to rely heavily on costly, time-intensive physical testing.*

*To address these challenges, this 2-day scientific exchange will bring together a diverse coalition of stakeholders from industry, academia, standards organizations, and the public sector. The event, co-hosted by the National Institute of Standards and Technology (NIST) and the Council on Ionizing Radiation Measurements and Standards (CIRMS) is designed to foster critical dialogue and collaboration around building the scientific infrastructure needed to elevate modeling and simulation into trusted components of sterilization workflows.*

*Participants will explore how rigorous practices from adjacent fields---most notably radiation therapy---can be adapted to meet the specific needs of sterilization. The exchange will examine current modeling approaches, validation techniques, and digital toolchains, and will identify technical gaps and barriers that hinder broader acceptance. Key topics include model verification and validation, uncertainty quantification, round-robin intercomparisons, traceability to standards, and the role of metrology in underpinning trustworthy simulation outputs.*

# Workshop Summary

## Goal

The following goals were highlighted during the introductory talks:

-   Assess...

-   Review best practices in model validation

-   Identify needs in fixture development, uncertainty quantification, cross validation

-   Explore how standards / guidance documents can support acceptance

-   Inform the next edition of the CIRMS needs report to help guide NISR priorities in this area

## Messages

The following messages were mentioned during the talks of the plenary sessions:

-   J. Meissner: We demonstrated the value of modelling long time ago (RPSMUG 2002, simu of CAPA \[Abbott\] in 2013) and stds are in place (ex: E2232-10 in 2000, ASTM E1649 \[now 51649\])

-   J. Meissner: Modelling can reduce time & cost for product design

-   S. Mickum:

    -   Modelling is used in many areas (flight simulator, aerodynamism, air quality, etc.) and help improve design / take right decision).

    -   In Medicine, it is used more & more (orthopedics, cardiology, etc.).

    -   Compared to traditional method, simulation allows cost effectiveness, Time efficiency, Safety & risk reduction, Richness of data & Insights.

    -   Regulatory bodies actively promotes & recognize the value of CM&S as part of the evidence package for device approval & clearance

-   P. Afshiri showed a great example of the use of modeling to get FDA clearance for the use of MRI on patient having metallic implants. Solving the problem would not have been possible w/o simulation

-   S. Mickum: Is modeling credible for its intended use?

-   S. Mickum: What tolerance are appropriate?

-   S. Mickum: Best practices :

    -   "Reporting of Computational Modeling Studies in Medical Device Submissions -- Guidance for Industry & FDA", 2016 ([Reporting of Computational Modeling Studies in Medical Device Submissions - Guidance for Industry and Food and Drug Administration Staff](https://www.fda.gov/media/87586/download))

    -   2 other reports mentioned by Spencer.

-   J. Logar: Collaboration with the regulators to decide on the acceptance criteria allow great time saving when it comes to demonstrate functional equivalence in an effort to reduce requalification (ex: Tyvek® from Dupont™).

-   J. Logar: Inactivation is an inaccurate science, It should not be hard to have confidence in modeling.

-   S. Mickum: The stds do not define the number of dosimeters in a dose mapping, while simulation allows to get dose at any point 🡺 one could reduce the \# of dose mappings and improve the final results.

-   In RT, the trust the simu (the dose is defined by the TP). The patient QA is not as accurate. It is just there to detect error! In RP, what is critical is to be sure of the transfer of the product into the modelling s/w (J. Logar).

-   D. Mihailidis: the Therapy Physics Committee (TPC) from AAPM achieves the following gools through its Subcommittees, Working Groups and Task Groups (TG):

    -   Improve accuracy and consistency of RT through development and publication of scientific, technical and educational documents

    -   Improve medical interventions through research and promote research in therapy applications of medical physics

    -   Provide guidance to outside agencies and organizations relative to the scientific and clinical interest of AAPM membership

    -   Remain aware of developments from and collaborate with outside organizations.

-   Regulator: the information required by the FDA depends on product type. For instance, the FDA is less demanding for Class II products than for class III products (where complete IQ, OQ, PQ data are requested).

-   Advice from FDA on how/what to present in the submission file:

    -   Say that you are not changing anything. Just taking advantage of the great tool.

    -   Show the protocol.

    -   Show you do not model anything different than what is being done.

    -   Show trends.

    -   Show uncertainties.

    -   Show what it would do to patient. Alos remember that the type/depth of info will drive the question from FDA ==\> do pre-discussion w/ FDA to clarify what should be shown in order to have a regulatory-technical discussion (and not a scientific discussion)!

-   Regulator: FDA claim they would be proactive, if we are in line and if we are confident in what we are simulating ==\> our confidence is important: "*You should build confidence with the regulator. To do so, the community should talk as one voice*!"

-   S. Mickum: RayXpert is validated. Validation includes benchmarking w/ MCNP6.2, GEANT4 and published scientific literature for accuracy

-   We should aim at functional equivalence (w/ well defined source)

-   About CT images for simulation:

    -   E. Carvan: Having on-line imaging would be a beautiful innovation

    -   Ayeh mentions a sensitivity analysis is important in EB (ex to see sensitivity to film packaging placement). Tobias highligths that this is not capture today w/ dosimetry!

-   J. Logar: Actual dose is way too conservative!

## Questions

The following questions were raised during the talks of the plenary sessions:

-   S. Mickum: Is modeling credible for its intended use?

-   S. Mickum: What tolerances are appropriate?

-   Group C: 5% tolerance in RT. Does it apply in RP?

-   Group C + J. Logar: What is important: accurate or credible model? Do we want an exact model or a functional equivalent model?

-   Group C: Can Simu be considered compliant w/o validation? Quid relative vs. absolute?

## Use of modelling

During the workshop, four cases were discussed where modeling could be helpful for the RP community. I gathered them in the following 2 x 2 matrix:

+---------------------------+-------------------------------------------------------------------------------------------------------------+---------------------------------------------------------------------------------+
|                           | Would not require regulatory approval / std changes in std                                                  | Would requires regulatory approval / std changes in std                         |
+===========================+=============================================================================================================+=================================================================================+
| **Product Design**        | -   Rapid iteration & failure detection 🡺 Reduce time-to-market + reduce cost (prototype, Case study, etc.) |                                                                                 |
+---------------------------+-------------------------------------------------------------------------------------------------------------+---------------------------------------------------------------------------------+
| **Product qualification** | -   PQ dose mapping: helps placing dose. Save time, more efficient 🡺 Improved patient safety                | -   Demonstrate functional equivalence in an effort to reduce requalification   |
|                           |                                                                                                             |                                                                                 |
|                           |                                                                                                             | -   PQ dose mapping: replace partly (or totally?) physical dose mappings by VDM |
+---------------------------+-------------------------------------------------------------------------------------------------------------+---------------------------------------------------------------------------------+

## Roadmap / list of tasks

The three working groups worked on an action plan. The define the tasks that would be needed to move forward and have CM&S efficiently used in the RP community. I collected the following list:

-   Why simulation? 🡺 What is the value proposition/benefits for the patient and for the businesses of...

    -   removing dosimetry ?

    -   getting next product being approved faster?

    -   all what I could do w/ modeling?

```{=html}
<!-- -->
```
-   Build **confidence for the regulator**

    -   **FDA: Talk as one voice**

    -   form a community of user.

    -   Aligned consensus.

    -   Phantoms,

```{=html}
<!-- -->
```
-   [Quantify uncertainty =\> Uncertainty mgt]{.mark}

-   [Phantom / std model]{.mark}

-   [Control of process:]{.mark}

    -   [What confidence in control? Need to show that you really understand each step]{.mark}

    -   [FDA does not only look at the perceived risk, but the perceived control]{.mark}

```{=html}
<!-- -->
```
-   Start w/ photons:

    -   Photons is mainly what we do today

    -   but the LT benefits maybe for EB

-   Technical translation

    -   Speak language everybody understand.

    -   Translate in simplistic terms

    -   Ex: BPSA

```{=html}
<!-- -->
```
-   Benchmarking / translation data:

    -   DP: inter-comparison on a std model. Tobias likes complex model that represents reality (ex: syringes instead of cylinder)

    -   Leo: BPSA model

-   Design process integration (simu for R&D)

-   [Modeling expertise: Competency? What needs to be a good modeler?]{.mark}

-   Lust of validated & approved tools

-   Bringing confidence

    -   COP or better: a program

    -   \>\< RT, they have accredited medical physicists.

-   Upfront integration

Work group A discussed the possible contribution of existing groups:

-   Universities

-   [The Irradiation Panel]{.mark}

    -   [Uncertainty mgt]{.mark}

    -   [Phantom / std model]{.mark}

    -   [Competency? What needs to be a good modeler?]{.mark}

    -   [Control of process -]{.mark}

-   KILMER (AAMI)

    -   JL doesn\'t believe there is much value there now (more focus on µ-biology)

-   CIRMS

    -   Get funding

    -   Benefits paper (white paper)

-   IIA / IAEA:

    -   Webinars to raise awareness

    -   Tech Doc

-   ASTM

    -   Collaboration w/ Panel

    -   From PQ to modelling. How do you demonstrate the control?

    -   Beam model

-   AAPM (same physics, comes from high energy. FDA confirms it could help)

    -   Technical translation

-   NIST:

    -   Control of the process / Traceability of the model

-   Radiation Research Society

-   ASME

Group A discussed also possible opportunities for funding:

-   NNSA

-   Consortium of companies (see benefits)

-   Dpt of congress

-   Other dedicated grant funding

## Next steps:

-   **J. Logar send an invitation to contribute to everyone: "Send your ideas. Do you want to contribute to one action item?"**

-   J. Logar commits to write a white paper around this WS

-   J. Logar leads the group to write the benefits.
