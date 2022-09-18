---
layout: archive
title: "Reading List"
permalink: /readinglist/
author_profile: true
---

This Website contains papers relevant to my research interest.

# All Papers (Classification according to Publication)

- **ISSTA 2022**  
  - [A Large-Scale Empirical Analysis of the Vulnerabilities Introduced by Third-Party Components in IoT Firmware](#a-large-scale-empirical-analysis-of-the-vulnerabilities-introduced-by-third-party-components-in-iot-firmware-issta-2022)
  - [An Empirical Study on the Effectiveness of Static C Code Analyzers for Vulnerability Detection](#an-empirical-study-on-the-effectiveness-of-static-c-code-analyzers-for-vulnerability-detection-issta-2022)
  - [BET: Black-Box Efficient Testing for Convolutional Neural Networks](#bet-black-box-efficient-testing-for-convolutional-neural-networks-issta-2022)
  - [Detecting Multi-sensor Fusion Errors in Advanced Driver-Assistance Systems](#detecting-multi-sensor-fusion-errors-in-advanced-driver-assistance-systems-issta-2022)
  - Efficient greybox fuzzing of applications in Linux-based IoT devices via enhanced user-mode emulation
  - LiRTest: augmenting LiDAR point clouds for automated testing of autonomous driving systems

- **PLDI 2022**
  - Finding typing compiler bugs
  - Odin: On-Demand Instrumentation with On-the-Fly Recompilation

- **ESEC/FSE 2022**
  - Fuzzing Deep-Learning Libraries via Automated Relational API Inference
  - Generating Realistic Vulnerabilities via Neural Code Editing: An Empirical Study
  - MOSAT: Finding Safety Violations of Autonomous Driving Systems Using Multi-Objective Genetic Algorithm
  - Scenario-based Test Reduction and Prioritization for Multi-Module Autonomous Driving Systems
  - Static Executes-Before Analysis for Event Driven Programs
  - Understanding Performance Problems in Deep Learning Systems
  
- **ASE 2022**  
  - B-AIS: An Automated Process for Black-box Evaluation of AI-enabled Software Systems against Domain Semantics
  - Boosting the Revealing of Detected Violations in Deep Learning Testing: A Diversity-Guided Method
  - LawBreaker: An Approach for Specifying Traffic Laws and Fuzzing Autonomous Vehicles
  - ThirdEye: Attention Maps for Safe Autonomous Driving Systems
  - Unveiling the Hidden Defection of DNN Testing with Decision-Based Metamorphic Oracle


- **ICSE 2022**
  - Adaptive Test Selection for Deep Neural Networks
  - A Grounded Theory Based Approach to Characterize Software Attack Surfaces
  - BeDivFuzz: Integrating Behavioral Diversity into Generator-based Fuzzing
  - DeepState: Selecting Test Suites to Enhance the Robustness of Recurrent Neural Networks
  - Demystifying the Dependency Challenge in Kernel Fuzzing
  - EAGLE: Creating Equivalent Graphs to Test Deep Learning
  - Evaluating and Improving Neural Program-Smoothing-based Fuzzing
  - Large-scale Security Measurements on the Android Firmware Ecosystem
  - Linear-time Temporal Logic guided Greybox Fuzzing
  - Muffin: Testing Deep Learning Libraries via Neural Architecture Fuzzing
  - MVD: Memory-Related Vulnerability Detection Based on Flow-Sensitive Graph Neural Networks
  - Nessie: Automatically Testing JavaScript APIs with Asynchronous Callbacks
  - PerfSig: Extracting Performance Bug Signatures via Multi-modality Causal Analysis

- **OOPSLA 2022**  
  - Coverage-guided tensor compiler fuzzing with joint IR-pass mutation  

- **S&P 2022**

- **NDSS 2022**

- **USENIX SEC 2022**

- **SANER 2022**


- **Others 2022**  


### A Large-Scale Empirical Analysis of the Vulnerabilities Introduced by Third-Party Components in IoT Firmware (ISSTA 2022)
* <img src="/files/images/pdf_24px.png">[Paper](/files/papers/A_large_scale_empirical_analysis_of_the_vulnerabilities_introduced_by_third_party_components_in_IOT_firmware.pdf)

**Abstract:** As the core of IoT devices, firmware is undoubtedly vital. Currently, the development of IoT firmware heavily depends on third-party components (TPCs), which significantly improves the development efficiency and reduces the cost. Nevertheless, TPCs are not secure, and the vulnerabilities in TPCs will turn back influence the security of IoT firmware. Currently, existing works pay less attention to the vulnerabilities caused by TPCs, and we still lack a comprehensive understanding of the security impact of TPC vulnerability against firmware.  
To fill in the knowledge gap, we design and implement FirmSec, which leverages syntactical features and control-flow graph features to detect the TPCs at version-level in firmware, and then recognizes the corresponding vulnerabilities. Based on FirmSec, we present the first large-scale analysis of the usage of TPCs and the corresponding vulnerabilities in firmware. More specifically, we perform an analysis on 34, 136 firmware images, including 11, 086 publicly accessible firmware images, and 23, 050 private firmware images from TSmart. We successfully detect 584 TPCs and identify 128, 757 vulnerabilities caused by 429 CVEs. Our in-depth analysis reveals the diversity of security issues for different kinds of firmware from various vendors, and discovers some well-known vulnerabilities are still deeply rooted in many firmware images. We also find that the TPCs used in firmware have fallen behind by five years on average. Besides, we explore the geographical distribution of vulnerable devices, and confirm the security situation of devices in several regions, e .g., South Korea and China, is more severe than in other regions. Further analysis shows 2, 478 commercial firmware images have potentially violated GPL/AGPL licensing terms.

### An Empirical Study on the Effectiveness of Static C Code Analyzers for Vulnerability Detection (ISSTA 2022)
* <img src="/files/images/pdf_24px.png">[Paper](/files/papers/An_empirical_study_on_the_effectiveness_of_static_C_code_analyzers_for_vulnerability_detection.pdf)
* **Abstract:** Static code analysis is often used to scan source code for security vulnerabilities. Given the wide range of existing solutions implementing different analysis techniques, it is very challenging to perform an objective comparison between static analysis tools to determine which ones are most effective at detecting vulnerabilities. Existing studies are thereby limited in that (1) they use synthetic datasets, whose vulnerabilities do not reflect the complexity of security bugs that can be found in practice and/or (2) they do not provide differentiated analyses w.r.t. the types of vulnerabilities output by the static analyzers. Hence, their conclusions about an analyzer’s capability to detect vulnerabilities may not generalize to real-world programs. In this paper, we propose a methodology for automatically evaluating the effectiveness of static code analyzers based on CVE reports. We evaluate five free and open-source and one commercial static C code analyzer(s) against 27 software projects containing a total of 1.15 million lines of code and 192 vulnerabilities (ground truth). While static C analyzers have been shown to perform well in benchmarks with synthetic bugs, our results indicate that state-of-the-art tools miss in-between 47% and 80% of the vulnerabilities in a benchmark set of real-world programs. Moreover, our study finds that this false negative rate can be reduced to 30% to 69% when combining the results of static analyzers, at the cost of 15 percentage points more functions flagged. Many vulnerabilities hence remain undetected, especially those beyond the classical memory-related security bugs.  

### BET: Black-Box Efficient Testing for Convolutional Neural Networks (ISSTA 2022)
* <img src="/files/images/pdf_24px.png">[Paper](/files/papers/BET_black_box_efficient_testing_for_convolutional_neural_networks.pdf)
* **Abstract:** It is important to test convolutional neural networks (CNNs) to
identify defects (e.g. error-inducing inputs) before deploying them in security-sensitive scenarios. Although existing white-box testing methods can effectively test CNN models with high neuron
coverage, they are not applicable to privacy-sensitive scenarios
where full knowledge of target CNN models is lacking. In this work, we propose a novel Black-box Efficient Testing (BET) method for CNN models. The core insight of BET is that CNNs are generally
prone to be affected by continuous perturbations. Thus, by gener-
ating such continuous perturbations in a black-box manner, we
design a tunable objective function to guide our testing process for thoroughly exploring defects in different decision boundaries of the target CNN models. We further design an efficiency-centric policy to find more error-inducing inputs within a fixed query budget. We conduct extensive evaluations with three well-known datasets and five popular CNN structures. The results show that BET significantly outperforms existing white-box and black-box testing methods considering the effective error-inducing inputs found in a fixed query/inference budget. We further show that the error-inducing inputs found by BET can be used to fine-tune the target model, improving its accuracy by up to 3%.

### Detecting Multi-sensor Fusion Errors in Advanced Driver-Assistance Systems (ISSTA 2022)
* <img src="/files/images/pdf_24px.png">[Paper](/files/papers/Detecting_multi_sensor_fusion_errors_in_advanced_driver_assistance_systems.pdf)
* <img src="/files/images/youdao_note_24px.png">[Reading Note](/file/notes/issta22Detecting.md)

* **Abstract:** Advanced Driver-Assistance Systems (ADAS) have been thriving and widely deployed in recent years. In general, these systems receive sensor data, compute driving decisions, and output control signals to the vehicles. To smooth out the uncertainties brought by sensor outputs, they usually leverage multi-sensor fusion (MSF) to fuse the sensor outputs and produce a more reliable understanding of the surroundings. However, MSF cannot completely eliminate the uncertainties since it lacks the knowledge about which sensor provides the most accurate data and how to optimally integrate the data provided by the sensors. As a result, critical consequences might happen unexpectedly. In this work, we observed that the popular MSF methods in an industry-grade ADAS can mislead the car control and result in serious safety hazards. We define the failures (e.g., car crashes) caused by the faulty MSF as fusion errors and develop a novel evolutionary-based domain-specific search framework, FusED, for the efficient detection of fusion errors. We further apply causality analysis to show that the found fusion errors are indeed caused by the MSF method. We evaluate our framework on two widely used MSF methods in two driving environments. Experimental results show that FusED identifies more than 150 fusion errors. Finally, we provide several suggestions to improve the MSF methods we study.

