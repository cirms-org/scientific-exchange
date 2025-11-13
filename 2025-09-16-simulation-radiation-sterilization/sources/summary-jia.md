**Simulation modeling** 

- **Current Practice**

  - **Beam energy and modality:** Most facilities use **4–10 MeV electron beams** either directly for irradiation or to generate bremsstrahlung x-rays.

    - **Electron beams are generally preferred** because they offer higher throughput and efficiency for bulk processing.

  - **Dosimetry methods:** Dose distribution is typically verified using **film** or **alanine**, placed around or within the phantom/pallet.

    - These measurements provide spatial mapping but may be limited in representing highly heterogeneous setups.

  - **Dose targets:** The operational goal is to achieve consistent dosing, with the **maximum dose capped at ~40 kGy** and the **minimum threshold at ~25 kGy**, ensuring regulatory compliance and effective sterilization while avoiding overexposure.

- **Modeling and Translation**

  - **Monte Carlo (MC) simulations** are widely considered the gold standard for predicting 3D dose distributions in complex geometries.

    - They provide confidence in accounting for scatter, heterogeneities, and secondary particle effects.

  - For practical adoption, there needs to be a **clear translation path**: demonstrating how MC modeling results can be systematically integrated into **industrial workflows**, validated against real-world measurements, and accepted by regulatory authorities.

- **Challenges, Concerns, and Areas of Improvement**

  - **Simulation configuration and flexibility:**

    - Each facility operates with **unique irradiation configurations** (beam energy, scanning patterns, conveyor geometry, shielding).

    - Simulation frameworks must allow **customizable setups** so results are relevant across sites.

  - **Beam model quality:**

    - Current practice often depends on **vendor-supplied beam models/data**, which may not capture real operational variability.

    - There is a need for **independent verification of accuracy and stability** of beam models over time.

    - A formal **commissioning process for the MC dose engine**—similar to clinical radiotherapy—would strengthen confidence.

  - **Phantom and material representation:**

    - Processing objects are highly heterogeneous, including **polymers, plastics, electronics, and packaging materials** etc.

    - Accurate geometry and material assignment is challenging:

    <!-- -->

    - **CAD files may not exist, or may be outdated/inaccurate.**

    - Simplifications may lead to deviations in predicted dose.

    <!-- -->

    - **CT imaging** could be used to capture more accurate geometry and density information, though feasibility and throughput remain questions.

  - **Geometry uncertainties:**

    - **Motion or shifting of objects** during conveyor transfer can alter dose delivery, which is not always accounted for in simulations.

  - **Physics modeling at heterogeneous interfaces:**

    - Dose near **material boundaries** is difficult to model due to **electron disequilibrium effects**.

    - Experimental measurement is also limited in such regions, as film or alanine may not fully represent small-scale variations.

    - This remains a critical source of uncertainty when validating models against measurements.

  

**Experience from Rad Onc** 

- **Modeling and Software**

  - **Material definition:** In clinical radiotherapy, careful consideration is given to patient anatomy and tissue composition. It is important knowing **to what extent accuracy in geometry and material properties truly impacts dose calculation outcomes**, enabling prioritization between detailed modeling and practical efficiency.

  - **Beam modeling:** Radiotherapy requires thorough **beam commissioning** to characterize effective beam properties, including **energy spectrum, fluence distributions, and contamination from secondary photons and electrons**. This process ensures models are not blindly dependent on vendor data but instead reflect measured clinical reality.

  - **Transport physics:** Accurate modeling of **electron transport at interfaces** is critical, especially in regions of disequilibrium such as air cavities or tissue–bone interfaces. Radiation oncology has developed methodologies to both calculate and experimentally validate these effects.

  - **Computational efficiency:** Clinical practice has benefited from **GPU-based, dedicated dose calculation engines** (work at JHU) to achieve near real-time dose computation without sacrificing accuracy. This experience demonstrates how advanced hardware/software co-design can bring Monte Carlo methods into routine workflows.

  - **User interface:** Radiotherapy software is designed to be used safely by **non-Monte Carlo experts**, with error-proof interfaces and guardrails to prevent misuse. This is critical to broaden access while maintaining accuracy and safety.

- **Commissioning**

  - Radiation oncology mandates **independent verification** of vendor-provided beam and geometry specifications before clinical use. Measurements with calibrated detectors are used to establish commissioning data sets that serve as the baseline for ongoing QA. This process underscores the need for rigorous commissioning in any dose modeling system.

- **QA**

  - Comprehensive QA protocols are embedded at **daily, monthly, and annual** intervals to ensure beam stability, system accuracy, and overall treatment safety.

  - QA equipment itself must be **regularly calibrated and verified**, ensuring consistency across time and between institutions.

  - **Dose traceability** is important, with ionization chambers and dosimeters calibrated against NIST-traceable standards, ensuring universal comparability and regulatory compliance.

- **Education and Training**

  - The field defines clear **qualifications for dose calculation and measurement personnel**, embodied in the role of the **Qualified Medical Physicist (QMP)**. This ensures that only properly trained professionals assume responsibility for critical tasks.

  - Standardized **accreditation and regulation pathways** exist for training programs (e.g., **CAMPEP**), professional practice (e.g., **ABR board certification**). Similarly, software and equipment are regulated through bodies such as the **FDA**.

- **AAPM Guidelines and Documents**

  - The **American Association of Physicists in Medicine (AAPM)** has produced an extensive library of task group (TG) reports and practice guidelines. These provide detailed recommendations for modeling, commissioning, QA, and education, serving as authoritative standards. Industrial irradiation efforts could similarly benefit from consensus documents developed by professional societies.

  - TG reports can be adapted

 

  

**Possible action items** 

- **Model Development**

  - Build a **prototype software platform**—simple but functional—to serve as a proof of principle.

  - Incorporate a **commissioning and QA framework** similar to clinical radiotherapy, demonstrating feasibility and reliability of dose modeling for industrial irradiation.

- **Use Cases**

  - Apply the developed model to show feasibility and advantages, **build business cases**, why we move towards this direction.

  - Apply the developed model to evaluate **uncertainties due to motion, geometry, positioning, and orientation**, and investigate what levels of uncertainty are acceptable versus achievable.

  - Perform **retrospective dose reconstruction** for products processed at one or more irradiation facilities to quantify dose variation in real-world practice.

    - Use results to identify **areas for improvement** (e.g., where modeling or process control is needed) and **areas where requirements can be relaxed** without compromising outcomes.

- **Delivery Monitoring / QA**

  - Leverage **x-ray projection imaging** of pallets/products during irradiation to reconstruct contents and detect **gross errors** such as incorrect orientation, major motion, or substitution of content.

  - Develop workflows for integrating these monitoring steps into **routine QA and process validation**.

- **Phantom Development for Commissioning and QA**

  - Design and fabricate **standard phantoms** for both commissioning and routine QA:

    - **Homogeneous phantom** (with a suitable reference material, TBD) containing embedded dosimeters/chambers to allow 3D dose verification, confirming beam modeling and dose calculation accuracy in a uniform medium.

    - **Layered phantom** with representative materials to validate dose calculation accuracy in heterogeneous geometries.

    - **Semi-realistic pallet phantom**, mimicking typical product composition and configuration, to enable **end-to-end system verification**.

- **Documentation and Regulation**

  - Conduct a **review of AAPM Task Group (TG) reports**, focusing on parallels between radiation oncology and industrial irradiation.

  - Develop a **comparative framework** that identifies which TG recommendations are directly applicable, which require adaptation, and where new guidance is needed.

  - Use findings to inform the creation of **regulatory and best-practice documents** that can be adopted by the field.

 
