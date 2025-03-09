---
title: "C-SCRM Checklist"
weight: 62
# bookFlatSection: false
# bookToc: true
# bookHidden: false
# bookCollapseSection: false
# bookComments: false
# bookSearchExclude: false
---

# Cybersecurity Supply Chain Risk Management Checklist
The actions listed below reflect the guidance from throughout this handbook. They have been re-organized and streamlined. Note, the activities below are not necessarily performed in order from top-to-bottom; some may need to happen concurrently. That said, governance considerations are typically needed at the outset to set scope and ensure leadership buy-in.

## Governance, Policies, Planning, and Risk Management
* Create a charter that outlines the governance mission, purpose, responsibilities, scope, and guidelines with respect to supply chain cybersecurity
    * Identify stakeholders from across the utility, and key suppliers, that could be affected by changes in third-party risk management (e.g., centralized procurement processes)
    * Use an outcome-oriented change management model to implement new processes and policies
* Perform risk assessment at an organizational level and on critical operational segments
    * Identify vendors for systems and services in critical operations
    * Identify severity and impact for individual risks and individual vendors
    * Implement risk treatments for identified risks
* Develop policies and procedures to manage existing supplier relationships and onboard new suppliers:
    * Adopt one or more international standards as source(s) for policy requirements (e.g., NIST Cybersecurity Framework version 2.0, ISO/IEC 27001, ISO/IEC  62443)
    * Tailor requirements in standards to organizational needs
    * Centralize procurement processes as appropriate
    * Develop RFP processes that define cybersecurity requirements for vendors and/or pre-qualify vendors
    * Include cybersecurity requirements and expectations in contractual terms and conditions, including clean consequences for failure to comply with these terms
    * Apply internal mitigation measures
* Develop and maintain an Incident Response Plan
    * Include key elements addressing roles and responsibilities, detection, containment, eradication, recovery, and communication plans
    * Consider threat scenarios that could impact critical systems/operations
    * Develop playbooks to respond to potential threats/incidents
    * Conduct tabletop exercises to test incident response plan and playbooks
    * Update incident response plan with lessons learned
## Asset Management
* Understand business processes and identify critical systems/operations
* Identify operational and business constraints
* Identify internal capabilities and gaps in capabilities needed to implement desired level of cyber security program
* Implement Defensible Architecture. Some key characteristics include:
    * Segmentation between IT and OT (Purdue Levels 5 and 4)
    * Multiple DMZs as appropriate to separate traffic between IT and OT (within Level 4)
    * Segmentation of all processes (in Level 2) from the site-wide supervisory (Level 3)
    * Segmentation between processes within OT environments (in Level 2)
    * Separate management services (e.g., AD) for IT and OT
* Implement Secure Remote Access / Cloud Access
    * Separate DMZs for remote access and cloud access as appropriate
    * 2-step authentication for humans
* Monitor OT network and physical power system 
    * Monitor OT networks, especially gateways/bottlenecks for anomalous user activity
    * Monitor physical power systems as essential data source for anomalous activity
* Periodic review of critical systems and security practices
    * Assess which systems are critical as the utility grows or evolves
    * Reconfigure network architecture to align with risk and capabilities

## Procurement Processes: Vendor Risk Management from Cradle to Grave
* Vendor Risk Assessment Components:
    * Evaluate the vendor’s cybersecurity strategy, awareness, and controls (note: an established questionnaire like the NATF Energy Sector Supply Chain Risk Questionnaire may be a useful starting point)
    * Assess the geographical location of developers and operations personnel to identify potential risks
    * Conduct checks to ensure there are no international sanctions or known vulnerabilities
    * Assess financial stability to ensure the vendor can perform as required
    * Evaluate operational risks, including the vendor’s business continuity and disaster recovery plans
    * Consider strategic risks, such as alignment with business goals
    * Assess transaction risks, including the vendor’s capacity to perform due to technological failure or human error
* Cybersecurity Risk Mitigation Measures for Individual Systems
    * Implement access controls, restrict access to authorized personnel, and enforce role-based access controls
    * Ensure sensitive information is encrypted using secure protocols
    * Conduct regular backups and store them securely
    * Keep all software and firmware updated with the latest security patches
    * Use next-generation firewalls and intrusion detection/prevention systems
    * Segment the network to limit the impact of potential attacks
    * Employ advanced threat detection and response solutions like EDR or XDR
    * Continuously monitor the infrastructure for potential threats using SIEM systems and other tools.
* Steps to Take Post-Implementation:
    * Update asset and systems inventories to reflect the new hardware and software
    * Review and update business continuity plans and incident response processes
    * Conduct annual risk audits with the vendor to maintain ongoing security and compliance
    * Ensure all critical data and system configurations are backed up and tested regularly
* Offboarding Considerations:
    * Understand the uninstallation process for the vendor’s software and hardware
    * Ensure all data is deleted according to retention policies and vendor site data destruction procedures
    * Update all inventories to reflect the removal of the vendor’s systems
    * Ensure a smooth transition to new vendors, if applicable
