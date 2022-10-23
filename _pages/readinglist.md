---
layout: archive
title: "Reading List"
permalink: /readinglist/
author_profile: true
---

This page contains papers relevant to my research interest.

# All Papers (Classification according to Publication)

- **ISSTA 2022**  
  - [A Large-Scale Empirical Analysis of the Vulnerabilities Introduced by Third-Party Components in IoT Firmware](#a-large-scale-empirical-analysis-of-the-vulnerabilities-introduced-by-third-party-components-in-iot-firmware-issta-2022)
  - [An Empirical Study on the Effectiveness of Static C Code Analyzers for Vulnerability Detection](#an-empirical-study-on-the-effectiveness-of-static-c-code-analyzers-for-vulnerability-detection-issta-2022)
  - [BET: Black-Box Efficient Testing for Convolutional Neural Networks](#bet-black-box-efficient-testing-for-convolutional-neural-networks-issta-2022)
  - [Detecting Multi-sensor Fusion Errors in Advanced Driver-Assistance Systems](#detecting-multi-sensor-fusion-errors-in-advanced-driver-assistance-systems-issta-2022)
  - [Efficient greybox fuzzing of applications in Linux-based IoT devices via enhanced user-mode emulation](#efficient-greybox-fuzzing-of-applications-in-linux-based-iot-devices-via-enhanced-user-mode-emulation-issta-2022)
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

- **CCS 2022**
  - What Your Firmware Tells You Is Not How You Should Emulate It: A Speciﬁcation-Guided Approach for Firmware Emulation


- **Other**
  - [Automatic Vulnerability Detection in Embedded Devices and Firmware: Survey and Layered Taxonomies](#automatic-vulnerability-detection-in-embedded-devices-and-firmware-survey-and-layered-taxonomies)  


### A Large-Scale Empirical Analysis of the Vulnerabilities Introduced by Third-Party Components in IoT Firmware (ISSTA 2022)
* <img src="../files/images/pdf_24px.png">[Paper](/files/papers/A_large_scale_empirical_analysis_of_the_vulnerabilities_introduced_by_third_party_components_in_IOT_firmware.pdf)

* **Abstract:** As the core of IoT devices, firmware is undoubtedly vital. Currently, the development of IoT firmware heavily depends on third-party components (TPCs), which significantly improves the development efficiency and reduces the cost. Nevertheless, TPCs are not secure, and the vulnerabilities in TPCs will turn back influence the security of IoT firmware. Currently, existing works pay less attention to the vulnerabilities caused by TPCs, and we still lack a comprehensive understanding of the security impact of TPC vulnerability against firmware.  
To fill in the knowledge gap, we design and implement FirmSec, which leverages syntactical features and control-flow graph features to detect the TPCs at version-level in firmware, and then recognizes the corresponding vulnerabilities. Based on FirmSec, we present the first large-scale analysis of the usage of TPCs and the corresponding vulnerabilities in firmware. More specifically, we perform an analysis on 34, 136 firmware images, including 11, 086 publicly accessible firmware images, and 23, 050 private firmware images from TSmart. We successfully detect 584 TPCs and identify 128, 757 vulnerabilities caused by 429 CVEs. Our in-depth analysis reveals the diversity of security issues for different kinds of firmware from various vendors, and discovers some well-known vulnerabilities are still deeply rooted in many firmware images. We also find that the TPCs used in firmware have fallen behind by five years on average. Besides, we explore the geographical distribution of vulnerable devices, and confirm the security situation of devices in several regions, e .g., South Korea and China, is more severe than in other regions. Further analysis shows 2, 478 commercial firmware images have potentially violated GPL/AGPL licensing terms.

### An Empirical Study on the Effectiveness of Static C Code Analyzers for Vulnerability Detection (ISSTA 2022)
* <img src="../files/images/pdf_24px.png">[Paper](/files/papers/An_empirical_study_on_the_effectiveness_of_static_C_code_analyzers_for_vulnerability_detection.pdf)

* **Abstract:** Static code analysis is often used to scan source code for security vulnerabilities. Given the wide range of existing solutions implementing different analysis techniques, it is very challenging to perform an objective comparison between static analysis tools to determine which ones are most effective at detecting vulnerabilities. Existing studies are thereby limited in that (1) they use synthetic datasets, whose vulnerabilities do not reflect the complexity of security bugs that can be found in practice and/or (2) they do not provide differentiated analyses w.r.t. the types of vulnerabilities output by the static analyzers. Hence, their conclusions about an analyzer’s capability to detect vulnerabilities may not generalize to real-world programs. In this paper, we propose a methodology for automatically evaluating the effectiveness of static code analyzers based on CVE reports. We evaluate five free and open-source and one commercial static C code analyzer(s) against 27 software projects containing a total of 1.15 million lines of code and 192 vulnerabilities (ground truth). While static C analyzers have been shown to perform well in benchmarks with synthetic bugs, our results indicate that state-of-the-art tools miss in-between 47% and 80% of the vulnerabilities in a benchmark set of real-world programs. Moreover, our study finds that this false negative rate can be reduced to 30% to 69% when combining the results of static analyzers, at the cost of 15 percentage points more functions flagged. Many vulnerabilities hence remain undetected, especially those beyond the classical memory-related security bugs.  

### BET: Black-Box Efficient Testing for Convolutional Neural Networks (ISSTA 2022)
* <img src="../files/images/pdf_24px.png">[Paper](/files/papers/BET_black_box_efficient_testing_for_convolutional_neural_networks.pdf)

* **Abstract:** It is important to test convolutional neural networks (CNNs) to
identify defects (e.g. error-inducing inputs) before deploying them in security-sensitive scenarios. Although existing white-box testing methods can effectively test CNN models with high neuron
coverage, they are not applicable to privacy-sensitive scenarios
where full knowledge of target CNN models is lacking. In this work, we propose a novel Black-box Efficient Testing (BET) method for CNN models. The core insight of BET is that CNNs are generally
prone to be affected by continuous perturbations. Thus, by gener-
ating such continuous perturbations in a black-box manner, we
design a tunable objective function to guide our testing process for thoroughly exploring defects in different decision boundaries of the target CNN models. We further design an efficiency-centric policy to find more error-inducing inputs within a fixed query budget. We conduct extensive evaluations with three well-known datasets and five popular CNN structures. The results show that BET significantly outperforms existing white-box and black-box testing methods considering the effective error-inducing inputs found in a fixed query/inference budget. We further show that the error-inducing inputs found by BET can be used to fine-tune the target model, improving its accuracy by up to 3%.

### Detecting Multi-sensor Fusion Errors in Advanced Driver-Assistance Systems (ISSTA 2022)
* <img src="../files/images/pdf_24px.png">[Paper](/files/papers/Detecting_multi_sensor_fusion_errors_in_advanced_driver_assistance_systems.pdf)
* <img src="../files/images/youdao_note_24px.png">[Reading Note](../files/notes/issta22Detecting.pdf)

* **Abstract:** Advanced Driver-Assistance Systems (ADAS) have been thriving and widely deployed in recent years. In general, these systems receive sensor data, compute driving decisions, and output control signals to the vehicles. To smooth out the uncertainties brought by sensor outputs, they usually leverage multi-sensor fusion (MSF) to fuse the sensor outputs and produce a more reliable understanding of the surroundings. However, MSF cannot completely eliminate the uncertainties since it lacks the knowledge about which sensor provides the most accurate data and how to optimally integrate the data provided by the sensors. As a result, critical consequences might happen unexpectedly. In this work, we observed that the popular MSF methods in an industry-grade ADAS can mislead the car control and result in serious safety hazards. We define the failures (e.g., car crashes) caused by the faulty MSF as fusion errors and develop a novel evolutionary-based domain-specific search framework, FusED, for the efficient detection of fusion errors. We further apply causality analysis to show that the found fusion errors are indeed caused by the MSF method. We evaluate our framework on two widely used MSF methods in two driving environments. Experimental results show that FusED identifies more than 150 fusion errors. Finally, we provide several suggestions to improve the MSF methods we study.

### Efficient greybox fuzzing of applications in Linux-based IoT devices via enhanced user-mode emulation (ISSTA 2022)
* <img src="../files/images/pdf_24px.png">[Paper](../files/papers/Efficient_Greybox_Fuzzing_of_Applications_in_Linux_Based_IOT_Devices_via_Enhanced_User_Mode_Emulation.pdf)
* <img src="../files/images/youdao_note_24px.png">[Reading Note](../files/notes/issta22Efficient.pdf)

* **Abstract:** Greybox fuzzing has become one of the most effective vulnerability discovery techniques. However, greybox fuzzing techniques cannot be directly applied to applications in IoT devices. The main reason is that executing these applications highly relies on specific system environments and hardware. To execute the applications in Linux-based IoT devices, most existing fuzzing techniques use full-system emulation for the purpose of maximizing compatibility. However, compared with user-mode emulation, full-system emulation suffers from great overhead. Therefore, some previous works, such as FirmAFL, propose to combine full-system emulation and user-mode emulation to speed up the fuzzing process. Despite the attempts of trying to shift the application towards user-mode emulation, no existing technique supports to execute these applications fully in the user-mode emulation.  
To address this issue, we propose EQUAFL, which can auto-
matically set up the execution environment to execute embedded
applications under user-mode emulation. EQUAFL first executes
the application under full-system emulation and observe for the key points where the program may get stuck or even crash during user-mode emulation. With the observed information, EQUAFL can migrate the needed environment for user-mode emulation. Then, EQUAFL uses an enhanced user-mode emulation to replay system calls of network, and resource management behaviors to fulfill the needs of the embedded application during its execution.  
We evaluate EQUAFL on 70 network applications from different
series of IoT devices. The result shows EQUAFL outperforms the state-of-the-arts in fuzzing efficiency (on average, 26 times faster than AFL-QEMU with full-system emulation, 14 times than FirmAFL). We have also discovered ten vulnerabilities including six CVEs from the tested firmware images.

### What Your Firmware Tells You Is Not How You Should Emulate It: A Speciﬁcation-Guided Approach for Firmware Emulation
* <img src="../files/images/pdf_24px.png">[Paper](../files/papers/What_your_firmware_tells_you_is_not_how_you_should_emulate_it.pdf)

* **Abstract:** Emulating firmware of microcontrollers is challenging due to the
lack of peripheral models. Existing work finds out how to respond
to peripheral read operations by analyzing the target firmware. This
is problematic because the firmware sometimes does not contain
enough clues to support the emulation or even contains misleading information (e.g., a buggy firmware). In this work, we propose
a new approach that builds peripheral models from the peripheral specification. Using NLP, we translate peripheral behaviors in
human language (documented in chip manuals) into a set of structured condition-action rules. By checking, executing, and chaining
them at runtime, we can dynamically synthesize a peripheral model
for each firmware execution. The extracted condition-action rules
might not be complete or even be wrong. We, therefore, propose incorporating symbolic execution to quickly pinpoint the root cause.
This assists us in the manual correction of the problematic rules.
We have implemented our idea for five popular MCU boards spanning three different chip vendors. Using a new edit-distance-based
algorithm to calculate trace differences, our evaluation against a
large firmware corpus confirmed that our prototype achieves much
higher fidelity compared with state-of-the-art solutions. Benefiting
from the accurate emulation, our emulator effectively avoids false positives observed in existing fuzzing work. We also designed a new dynamic analysis method to perform driver code compliance checks against the specification. We found some non-compliance which we later confirmed to be bugs caused by race conditions.

### Automatic Vulnerability Detection in Embedded Devices and Firmware: Survey and Layered Taxonomies
* <img src="../files/images/pdf_24px.png">[Paper](../files/papers/Automatic_Vulnerability_Detection_in_Embedded_Devices_and_Firmware_Survey_and_Layered_Taxonomies.pdf)

* **Abstract:** In the era of the internet of things (IoT), software-enabled inter-connected devices are of paramount impor-
tance. The embedded systems are very frequently used in both security and privacy-sensitive applications.
However, the underlying software (a.k.a. firmware) very often suffers from a wide range of security vulnerabilities, mainly due to their outdated systems or reusing existing vulnerable libraries; which is evident by the
surprising rise in the number of attacks against embedded systems. Therefore, to protect those embedded sys-
tems, detecting the presence of vulnerabilities in the large pool of embedded devices and their firmware plays
a vital role. To this end, there exist several approaches to identify and trigger potential vulnerabilities within
deployed embedded systems firmware. In this survey, we provide a comprehensive review of the state-of-the-
art proposals, which detect vulnerabilities in embedded systems and firmware images by employing various
analysis techniques, including static analysis, dynamic analysis, symbolic execution, and hybrid approaches.
Furthermore, we perform both quantitative and qualitative comparisons among the surveyed approaches.
Moreover, we devise taxonomies based on the applications of those approaches, the features used in the liter-
ature, and the type of the analysis. Finally, we identify the unresolved challenges and discuss possible future
directions in this field of research.

### Nessie: Automatically Testing JavaScript APIs with Asynchronous Callbacks
* <img src="../files/images/pdf_24px.png">[Paper](../files/papers/Nessie_automatically_testing_JavaScript_APIs_with_asynchronous_callbacks.pdf)
* <img src="../files/images/youdao_note_24px.png">[Reading Note](../files/notes/icse22nessie.md)

* **Abstract:** Previous algorithms for feedback-directed unit test generation iter-
atively create sequences of API calls by executing partial tests and
by adding new API calls at the end of the test. These algorithms
are challenged by a popular class of APIs: higher-order functions
that receive callback arguments, which often are invoked asyn-
chronously. Existing test generators cannot effectively test such
APIs because they only sequence API calls, but do not nest one call
into the callback function of another. This paper presents Nessie,
the first feedback-directed unit test generator that supports nesting
of API calls and that tests asynchronous callbacks. Nesting API calls
enables a test to use values produced by an API that are available
only once a callback has been invoked, and is often necessary to
ensure that methods are invoked in a specific order. The core con-
tributions of our approach are a tree-based representation of unit
tests with callbacks and a novel algorithm to iteratively generate
such tests in a feedback-directed manner. We evaluate our approach
on ten popular JavaScript libraries with both asynchronous and
synchronous callbacks. The results show that, in a comparison with
LambdaTester, a state of the art test generation technique that only
considers sequencing of method calls, Nessie finds more behavioral
differences and achieves slightly higher coverage. Notably, Nessie
needs to generate significantly fewer tests to achieve and exceed
the coverage achieved by the state of the art.

