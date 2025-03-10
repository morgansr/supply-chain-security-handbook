---
title: "Coordinating with Hardware/Software Vendors"
weight: 52
# bookFlatSection: false
# bookToc: true
# bookHidden: false
# bookCollapseSection: false
# bookComments: false
# bookSearchExclude: false
---

# Coordinating Cybersecurity Risk Management with Hardware/Software Vendors

## Webinar
{{< youtube P6-aSjgBXZc >}}

### Presenters
* **Claudia Iannazzo**, Catalisto
* **Sokol Mukaj**, KESH

## Summary
Utilities and other organizations could fall victim to a supply chain attack through no fault of their own as demonstrated in March 2023 by the 3CX supply chain attack (see call out box below). Rather than focusing on how to avoid a supply chain attack, utilities should focus on how to quickly detect and fully recover from such an attack by taking steps throughout the lifecycle of the relationship with the vendor from procurement and selection, during deployment, and through to offboarding. Best practices in coordinating cybersecurity risk management with vendors are exemplified by KESH, the Albania Power Corporation, which operates nearly 80% of the generation capacity, primarily from large hydropower plants, as well as guarantees the security of the Albanian energy system through balancing energy and auxiliary services. KESH implemented several advancements to its cybersecurity program through a program supported by USAID and carried out by Catalisto. 

Their advancement began with a detailed specification criteria for the type of technology solution that KESH needed, including a mix of software and hardware. The second step was to issue the RFP to a selection of vendors. KESH had selected about 70 vendors of widely varying sizes from the large, established companies to smaller ones. The broad vendor pool gave them a better chance at finding the best pricing. Moreover, multiple responses identified useful ideas and approaches that could potentially be adopted by the eventual selected vendor. They compiled the responses in an Excel spreadsheet to analyze them and apply the scoring rubric, leading to a vendor recommendation for KESH’s consideration.

{{% hint info %}}
**3CX Supply Chain Attack Example**
{.center}

In March 2023, an employee of 3CX, a company that provides VOIP software, downloaded a compromised version of a futures trading software, X_Trader to their personal computer. While this compromised version of X_Trader appeared legitimate and came directly from the software developer, it had a malware installer.

Two days later, 3CX recorded an attacker using that employee’s credentials to access the company’s VPN. The attacker then loaded a dynamic link library (DLL) payload into 3CX’s Electron Desktop Application corrupting it such that when it executes on one of 3CX’s clients’ machines, instead of querying a legitimate location for the DLL, it looked for the compromised version. The compromised DLL would then allow the attackers to download additional malware onto the clients’ machines. Note that, like the X_Trader software, the compromised version of 3CX’s Electron Desktop Application appeared to be legitimate because the compromise had occurred prior to the legitimate distribution channels for that software.

The attackers were able to gain access to a significant portion of 3CX’s customers; victims included at least a US energy operator and a European energy operator. This attack is one of the first examples of a supply chain attack (through X_Trader), which lead to a second supply chain attack (through the Electron Desktop Application).
{{% /hint %}}

## Information Request through the RFP
Utilities collect critical information from the vendor either through the RFP response process or through the negotiation process. Utilities should understand whether the vendor themselves uses third party providers or outsourcing to deliver the software to the utility. Moreover, the location of those second-tier suppliers should be known, because they might be located in countries that increase the geopolitical risk of acquiring the product or service. That is, utilities should understand where the vendor’s support team and/or development team is located. Another essential piece of information in contact information for a CISO such that the utility can reach someone in case of an incident. 

Additionally, utilities should have a decent understanding of the solution description and capabilities. Utilities should understand the solution architecture, including the hardware needs, integration needs, deployment environment (e.g., on-premises or cloud-based), and whether it contains open-source resources. Data flows through the product are also important. Utilities should determine what data of theirs will go to the product or service as well as where the service might be sending data. Similarly, where the data is stored, how long it is kept, and how it is backed up should all be known. These details should align with the needs of the utility as described in the RFP. Finally, utilities should ask about multi-factor authentication for administrators at a minimum and for additional users if applicable. Many vendors do not yet support MFA, so utilities should ask.

## Response Packages
For some vendors, the NATF questionnaire may be excessive and a barrier to responding to the RFP if the questionnaire is a part of it. Table 5 below lists six questions that may be useful without being too burdensome on the vendor along with some guidance on why to ask the question and how to interpret responses.

<table>
    <tr>
        <th>Question</th>
        <th>Response Interpretation</th>
    </tr>
    <tr>
        <td>1.	Do you have any security related certifications/ standards you commit to (e.g. ISO27001, SOC Type II, NIST 800-171, CMMC etc.) and if so describe whether you are independently audited to the standard or self-certified to that standard.</td>
        <td>The specific standard is not necessarily important so much as the vendor’s level of maturity and therefore level of risk that the procuring utility should plan for.</td>
    </tr>
    <tr>
        <td>2.	How many successful cybersecurity attacks has your organization experienced in the last 2 years? Successful means the attacker was able to gain unauthorized access to systems or information (including solution source code).</td>
        <td>Most companies have experienced some type of breach, so an answer of “zero” may be suspect. It could indicate that the vendor has poor detection or that they are unwilling to be forthcoming.</td>
    </tr>
    <tr>
        <td>3.	When was the last time your technical solution was manually penetration tested? (meaning human specialists were used to systematically identify vulnerabilities, navigate the application/ system and attempt to exploit vulnerabilities)</td>
        <td rowspan="2">Penetration tests, whether focused on a technical solution or an entire organization, are more involved than an automated vulnerability scan. These questions can indicate the vendor’s sophistication and how seriously they take their own cybersecurity capabilities.</td>
    </tr>
    <tr>
        <td>4.	When was the last time your organization was manually penetration tested? (meaning human specialists were used to systematically identify vulnerabilities, navigate the application/ system and attempt to exploit vulnerabilities)</td>
    </tr>
    <tr>
        <td>5.	Will you agree to disclose the name, nationalities and countries of residence of all personnel involved in implementation of the solution on our systems (that are of national importance)?</td>
        <td>As critical energy infrastructure, it may be inappropriate for citizens of countries with problematic relationships with the utility’s country to support the project.</td>
    </tr>
    <tr>
        <td>6.	Will you agree to sign a mutual NDA with the operator to ensure any information disclosed to you during implementation or otherwise is kept in strict confidence?</td>
        <td>Reputable vendors will be willing to sign an NDA. Utilities should not rely solely on the procurement contract, so a separate NDA is worthwhile.</td>
    </tr>
</table>

## Compliance Checks
Utilities should conduct checks on their suppliers and their products using one or more public databases before signing a contract to look for sanctions or known vulnerabilities. Three useful resources include the Sanctions List Search, the UN Consolidated List, and the NIST National Vulnerability Database.

* [U.S. Treasury, Office of Foreign Assets Control, Sanctions List Search](https://sanctionssearch.ofac.treas.gov/)  
Utilities can check the name of the company, the current leadership, and or the company owner or founder with this database of US sanctions.

* [United Nations Security Council Consolidated List](https://main.un.org/securitycouncil/en/content/un-sc-consolidated-list)  
The UN Security Council Consolidated list contains information on international sanctions that utilities should be aware of before signing a contract.

* [NIST National Vulnerability Database (NVD)](https://nvd.nist.gov/)  
The NVD contains a list of public vulnerabilities across many different products. Utilities can check the product they are procuring, find vulnerabilities, look at the severity score for the vulnerability, and potentially find a vendor advisory with additional information and patch if available.

## Vendor Negotiations
Once the utility has selected a vendor, they will typically enter negotiations to finalize the contract. Utilities should clarify any remaining questions about the vendor’s response to the RFP. In addition, utilities should check the vendor’s references, preferably in a similar industry (e.g., other energy operators). Rather than ask whether the vendor is good or bad, ask process-oriented questions like “what are the things we should do to get the best value from the vendor?” or “Can you explain the implementation process the vendor took you through?” to get more insightful responses. 

This negotiations phase may uncover changes that should be included in writing in the contract and statement of work. 

Finally, utilities should conduct a vendor risk assessment, which can consider many different dimensions beyond just cybersecurity risk specifically. Utilities can consider compliance risk, reputational risk, credit/ financial risk, operational risk, strategic risks, and transaction risks. 

## Implementation Phase
During implementation, utilities should use a documented Implementation Plan to capture all the details of the implementation. This should be a living document that is updated throughout the implementation, including a final update at the end of the project to capture the final details. This document becomes a record of how the implementation was done and what decisions were made and why. An example Table of Contents for an implementation plan is shown in Figure 19.

In addition to the vendor risk assessment, utilities should conduct a risk assessment specific to the implementation of the vendor’s product within the utility’s network. The risk assessment will identify specific risks related to the implementation. The utility can develop recommendations and measures that the vendor should take prior to implementation. For example, if the vendor requires remote access for maintenance, then they must implement (or agree to utility implemented) secure remote access in line with zero-trust principles. 

![Figure 19. Example Table of Contents from KESH's Implementation Plan](figures/100_Implementation_Plan_TOC.png)
Figure 19. Example Table of Contents from KESH's Implementation Plan
{.figure-caption}

## Post Implementation Phase & Offboarding
Utilities should conduct vendor management beyond the implementation phase. Continuous post-implementation management includes regular security audits and compliance checks to ensure that the implementation aligns with the requirements and that controls are functioning as intended. Utilities should keep a detailed log of interactions and changes to ensure traceability. Finally, utilities should establish clear communication channels with vendors for reporting and resolving issues.

Eventually, the utility may decide to pursue another solution and therefore will need to offboard a previous vendor. Utilities should document a thorough offboarding process to prevent data leakage and maintain security even after the relationship. The utility should understand the uninstallation process for software and hardware. The vendor should attest that data destruction policies are followed at the vendor’s site. Finally, the utility should update its asset and systems inventories to reflect the removal of vendor systems.

## Vendor Risk Management from Cradle to Grave
### Vendor Risk Assessment Components
* Evaluate the vendor’s cybersecurity strategy, awareness, and controls.
* Assess the geographical location of developers and operations personnel to identify potential risks.
* Conduct checks to ensure there are no international sanctions or known vulnerabilities.
* Assess financial stability to ensure the vendor can perform as required.
* Evaluate operational risks, including the vendor’s business continuity and disaster recovery plans.
* Consider strategic risks, such as alignment with business goals.
* Assess transaction risks, including the vendor’s capacity to perform due to technological failure or human error.
### Cybersecurity Risk Mitigation Measures
* Implement access controls, restrict access to authorized personnel, and enforce role-based access controls.
* Ensure sensitive information is encrypted using secure protocols.
* Conduct regular backups and store them securely.
* Keep all software and firmware updated with the latest security patches.
* Use next-generation firewalls and intrusion detection/prevention systems.
* Segment the network to limit the impact of potential attacks.
* Employ advanced threat detection and response solutions like EDR or extended detection and response (XDR).
* Continuously monitor the infrastructure for potential threats using SIEM systems and other tools.
### Steps to Take Post-Implementation
* Update asset and systems inventories to reflect the new hardware and software.
* Review and update business continuity plans and incident response processes.
* Conduct annual risk audits with the vendor to maintain ongoing security and compliance.
* Ensure all critical data and system configurations are backed up and tested regularly.
### Offboarding Considerations
* Understand the uninstallation process for the vendor’s software and hardware.
* Ensure all data is deleted according to retention policies and vendor site data destruction procedures.
* Update all inventories to reflect the removal of the vendor’s systems.
* Ensure a smooth transition to new vendors, if applicable.

## Additional Resources
* U.S. Treasury, Office of Foreign Assets Control, [Sanctions List Search](https://sanctionssearch.ofac.treas.gov/)
* United Nations Security Council [Consolidated List](https://main.un.org/securitycouncil/en/content/un-sc-consolidated-list)
* NIST [National Vulnerability Database](https://nvd.nist.gov/)
* Catalisto, Vendor Risk Analysis Template (xlsx)



