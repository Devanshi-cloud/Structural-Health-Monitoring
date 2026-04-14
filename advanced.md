# Integrating Emerging Sensing Technologies with Bio-Waste-Based Sustainable Concrete for Advanced SHM  

## 1.  Why a New Approach Is Needed  
Conventional piezoelectric (PZT) sensors provide high sensitivity but suffer from durability loss under long-term loading, high temperature, and harsh concrete environments, and their deployment often requires extensive wiring and calibration [1]. When paired with eco-friendly binders such as calcined clamshell or eggshell powders, which introduce additional chemical and micro-structural variability, these limitations become more pronounced [2][3].

## 2.  Advanced Sensing Technologies Beyond PZT  

### 2.1  Fiber-Optic Sensors (FBG & Brillouin Distributed Sensing)  
- **Fiber-Bragg Grating (FBG)** sensors can be embedded directly in concrete to monitor strain, temperature, and corrosion with sub-microstrain resolution and are resistant to electromagnetic interference [4].  
- **Brillouin Distributed Fiber-Optic Sensors (B-DOFS)** enable kilometre-scale strain/temperature profiling, making them ideal for large structural elements such as bridges or slabs. Recent work demonstrates their ability to capture both global and localized damage, including crack initiation during fire exposure [5].  
- Embedding strategies using epoxy-sheet encapsulation or 3D-printed resin carriers have proven to preserve sensor integrity while maintaining concrete workability [6].

### 2.2  Self-Sensing Cementitious Composites  
- **Graphene nanoplatelets (GNPs)** added at 4-6 wt % impart a linear piezoresistive response that can be read directly from the concrete matrix, eliminating separate wiring. The approach also improves compressive strength up to a threshold, offering a dual mechanical-sensing benefit [7].  
- **Multi-walled carbon nanotubes (MWCNTs)** at ≤0.1 wt % enhance both flexural strength and intrinsic electrical conductivity, enabling real-time monitoring of strain and damage through simple resistance measurements. Field trials on railway sleepers have shown reliable defect detection under service loads [8].

### 2.3  Acoustic Emission (AE)  
Automated high-precision AE algorithms can locate crack sources with ten-fold higher spatial resolution than manual processing, and are scalable to meter-scale concrete beams. The software supports real-time moment-tensor inversion, offering insight into fracture mechanisms that complement strain-based sensors [9].

### 2.4  Hybrid Piezoelectric Strategies  
Recent reviews highlight the use of flexible mica-based PZT films, multi-orientation arrays, and electro-mechanical impedance (EMI) techniques combined with machine-learning autoencoders to reduce false alarms and extend sensor life under high-temperature conditions [1].

## 3.  Linking Sensors to Sustainable Bio-Waste Concrete  

| Sustainable Binder | Key Mechanical Effect | Compatible Sensor Strategy |
|--------------------|----------------------|----------------------------|
| **Calcined clamshell powder** - high CaO content improves early-age strength but may alter pore structure [2] | Slightly higher early compressive strength; potential for increased alkalinity | Fiber-optic strain sensors embedded during casting (epoxy-sheet method) to monitor early-age shrinkage and carbonation [6] |
| **Calcined eggshell powder** - provides pozzolanic activity and reduces clinker demand [3] | Comparable 28-day strength with reduced CO₂ footprint; improved durability | Self-sensing GNP or MWCNT additives can be co-dispersed with eggshell powder, enabling intrinsic resistance-based monitoring without extra wiring [7][8] |

Embedding fiber-optic or nanomaterial sensors does not significantly interfere with the pozzolanic reactions of these waste powders, provided that the filler dispersion is controlled (e.g., surfactant-assisted mixing for CNTs).

## 4.  AI/ML, Data-Driven SHM, and Digital Twins  

- **Multimodal Data Fusion**: Combining vibration, strain (FBG or self-sensing resistance), AE, and environmental data improves defect classification. Studies show that lack of benchmark datasets hampers model generalisation; creating open, multimodal repositories for bio-waste concrete is a priority [10][11].  
- **Edge-Enabled Analytics**: Low-power microcontrollers equipped with neural-processing units can run quantised CNNs on raw vibration or acoustic signatures, delivering >99 % crack detection accuracy locally and reducing cloud bandwidth [12].  
- **Digital Twin Integration**: Real-time sensor streams feed a high-fidelity FEM model that updates strain, temperature, and damage fields continuously. Pilot bridge projects have demonstrated predictive maintenance by coupling digital twins with weigh-in-motion data, achieving early warning of overload events [13].

## 5.  Wireless, Low-Power IoT Solutions  

- **LoRaWAN** offers sub-USD 6 k total cost of ownership for 100-node deployments over five years, with battery life of 5-10 years and excellent penetration through concrete and steel .  
- **BLE Mesh** and **ZigBee** are suitable for high-data-rate vibration nodes, while **NB-IoT/LTE-M** can provide cellular backup for critical infrastructure.  
- Energy-harvesting techniques (vibration-based piezoelectric harvesters) can power ultra-low-power accelerometers, extending node lifetimes without battery replacement [14].

## 6.  Current Gaps & Under-Explored Opportunities  

1. **Durability of Sensors in Bio-Waste Concrete** - Long-term chemical interaction between high-alkali waste binders and embedded optical fibers or nanomaterial networks remains insufficiently studied.  
2. **Standardised Calibration for Self-Sensing Concrete** - No universally accepted conversion from resistance change to strain for GNP- or CNT-modified mixes, especially when waste powders modify moisture transport.  
3. **Multimodal Fusion Frameworks for Green Concrete** - Existing AI models are trained on conventional concrete datasets; transferring them to waste-based mixes requires domain-adaptation techniques.  
4. **Scalable Embedding Techniques** - While epoxy-sheet encapsulation works for laboratory beams, scalable methods for precast or in-situ casting (e.g., 3D-printed sensor housings) need validation.  
5. **Lifecycle Assessment of Sensor-Concrete Systems** - Integrated LCA that accounts for sensor material (glass fiber, carbon nanomaterials) and waste-binder benefits is rare, limiting ESG quantification.

## 7.  Suggested Research Directions  

| Direction | Rationale | Example Implementation |
|-----------|-----------|------------------------|
| **Hybrid Fiber-Optic / Self-Sensing Matrices** | Leverages the distributed coverage of DOFS while exploiting intrinsic resistance of GNP/CNT networks for redundancy. | Coat a single optical fiber with a thin CNT-infused cement sheath; use FBG for temperature, resistance for strain. |
| **Edge-AI for Early-Age Monitoring** | Early shrinkage and carbonation are critical in waste-based mixes; on-site inference reduces data latency. | Deploy Raspberry Pi-based nodes running a 1-D convolutional autoencoder on EMI data to flag abnormal stiffness evolution [1]. |
| **LoRaWAN-Backed Digital Twin Platform** | Low-cost connectivity enables city-scale deployment; digital twin provides predictive maintenance for municipal bridges built with eco-concrete. | Integrate LoRaWAN nodes measuring FBG strain, AE counts, and resistance into a cloud-hosted FEM model updated every 10 min. |
| **Standardised Test Protocols for Bio-Concrete Sensors** | Facilitates comparison across labs and accelerates adoption. | Follow the early-age strain embedding protocol (epoxy-sheet method) and publish a benchmark dataset of strain, temperature, and resistance for clamshell/eggshell mixes. |
| **Life-Cycle Impact Modelling** | Quantifies net sustainability benefit of sensor-enhanced green concrete. | Combine LCA of clamshell/eggshell substitution (≈30 % cement reduction) with embodied energy of optical fibers and CNTs, using the cost-benefit framework for sensor networks [15]. |

## 8.  Concluding Outlook  

The convergence of **distributed fiber-optic sensing**, **nanomaterial-based self-sensing concrete**, **high-resolution acoustic emission**, and **AI-driven digital twins** creates a pathway to overcome the durability and scalability limits of traditional PZT systems, especially when paired with **calcined clamshell and eggshell powders**. By addressing the identified gaps-sensor durability in alkaline waste matrices, calibration standards, multimodal AI integration, and lifecycle impact-future research can deliver robust, low-cost, and environmentally responsible SHM solutions ready for large-scale infrastructure deployment.

---

### Sources
- [1] https://link.springer.com/article/10.1007/s44416-026-00046-8
- [2] https://www.researchgate.net/publication/389312455_Clam_Shell_Powder_as_Cement_Substitution_in_Concrete_Production
- [3] https://link.springer.com/article/10.1007/s44416-025-00021-9
- [4] https://pmc.ncbi.nlm.nih.gov/articles/PMC7472180/
- [5] https://pmc.ncbi.nlm.nih.gov/articles/PMC8347898/
- [6] https://pmc.ncbi.nlm.nih.gov/articles/PMC8235537/
- [7] https://pmc.ncbi.nlm.nih.gov/articles/PMC10459810/
- [8] https://pmc.ncbi.nlm.nih.gov/articles/PMC12196629/
- [9] https://infoscience.epfl.ch/bitstreams/9c67895a-b741-4d07-a408-e324c780f067/download
- [10] https://www.mdpi.com/2076-3417/15/9/4855
- [11] https://iopscience.iop.org/article/10.1088/1361-6501/ae3abb
- [12] https://www.encardio.com/blog/wireless-sensor-networks-structural-health-monitoring-guide
- [13] https://www.civilengineeringjournals.com/jcea/article/43/6-1-15-841.pdf
- [14] https://pmc.ncbi.nlm.nih.gov/articles/PMC10611078/
- [15] https://pmc.ncbi.nlm.nih.gov/articles/PMC6068495/
