
# On the Edge of Security: Threat-Driven Pentest of KubeEdge with ESSecA

This repository contains the resources for the paper "Formal Graph-Based Approach for Cyclical Automated Penetration Testing in IoT systems". The tool used to generate the Threat Model, and the Attack Plan is developed by our team and is available at [Pennet](https://pennet.vseclab.it/).

## Authors
- [Felice Moretta](felice.moretta@unicampania.it)
- [Umberto Barbato](umberto.barbato@unicampania.it)
- [Massimiliano Rak](massimiliano.rak@unina.it)
- [Daniele Granata](daniele.granata@uniparthenope.it)

## Abstract

Modern IT infrastructures require systematic security assessment approaches. However, ensuring model correctness and completeness in automated security evaluation remains challenging, particularly when new information emerges during penetration testing. This paper addresses these challenges by extending the ESSecA methodology with formal model validation and cyclical refinement capabilities.
We present a formal representation of MACM (Multi-purpose Application Composition Model). It is formalized as a property graph model, including syntactic and semantic constraints. 
The MACM formalization enables automated validation through Cypher queries in Neo4j, ensuring model correctness throughout the assessment lifecycle.
The methodology integrates a cyclical refinement process where penetration testing outcomes progressively enhance the system model, leading to more precise threat modeling and improved penetration test planning in subsequent iterations. This iterative approach addresses the typical limitations of grey-box penetration testing, where testers have incomplete system visibility.
We demonstrate the approach through two case studies: the eWeLink IoT ecosystem, showcasing the modeling capabilities of MACM, and the JetRacer autonomous vehicle platform, illustrating the complete cyclical methodology. The JetRacer evaluation identified 92 potential threats with 74 corresponding penetration tests, culminating in the successful execution of an HTTP session hijacking attack through five iterative cycles.

## Contents
- The *JetRacer MACM* folder contains the formal models of the JetRacer case study, created using the MACM (Multi-purpose Application Composition Model) formalism. MACM utilizes the Cypher query language to describe the system, enabling comprehensive security analysis. There are three versions of the model, each representing a different stage of the iterative refinement process, obtained by applying the ESSecA cyclical methodology.
- The *eWeLink MACM* folder contains the formal models of the eWeLink case study.
- [JetRacer_threat_model.xlsx](JetRacer_threat_model.xlsx): This spreadsheet documents the threat model developed during the threat modeling phase of the JetRacer case study.
- [JetRacer_attack_plan.xlsx](JetRacer_attack_plan.xlsx): The attack plan used in the pentest of the JetRacer case study.