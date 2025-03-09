---
title: "Managing Cybersecurity Risks in a Rapidly Expanding Electric Grid"
weight: 43
# bookFlatSection: false
# bookToc: true
# bookHidden: false
# bookCollapseSection: false
# bookComments: false
# bookSearchExclude: false
---

# Managing Cybersecurity Risks in a Rapidly Expanding Electric Grid

## Webinar

{{< youtube KfGkDP8mHdI >}}

### Presenters
* **Anuj Sanghvi**, NREL
* **Ginger Wright**, INL

## Summary
Energy systems around the world are evolving across several dimensions, which may increase complexity in risk in addition to delivering the promised benefits. Two major changes include (1) the shift to more of a “prosumer” model where stakeholders that were formally just energy consumers are becoming energy producers as well, and (2) the evolving ownership models for generation resources. For example, homeowners or a third party may own the residential solar PV system, but an aggregator may have some level of control over that resource in addition to the distribution utility. The move from traditional centralized grid to more distributed energy resources brings with it complexity, especially at the grid edge. Energy is no longer just consumed, but rather it is generated, stored, managed, and traded, as shown in Figure 17 below. Doing so requires complex communication networks, which increases potential cyber vulnerabilities. 

![Figure 17. The evolving grid includes more communications and active participation from more stakeholders.](/figures/080_evolving_grid.png)  
Figure 17. The evolving grid includes more communications and active participation from more stakeholders.
{.figure-caption}

## Distributed Energy Resources – Cybersecurity Framework
DER, like solar systems, wind systems, battery energy storage systems, and even electric vehicle charging equipment, are equipped with complex, data-driven communications networks to connect with the energy grid. These sophisticated devices often interact with legacy equipment that was not designed with security in mind. The growing number of devices that support DER can increase the number of access points outside a utility’s administrative control. Unauthorized access to these systems could destabilize the local distribution system.

The National Renewable Energy Laboratory (NREL) developed the Distributed Energy Resources – Cybersecurity Framework (DER-CF) to help organizations assess and mitigate gaps in their cybersecurity posture for DER. The DER-CF covers key areas such as governance, technical management, and physical security. It offers a publicly accessible interactive version (hosted at dercf.nrel.gov) that provides tailored assessments, detailed results, and recommended actions for improving cybersecurity at individual sites.

The DER-CF is based on the U.S. Department of Energy’s Cybersecurity Capability Maturity Model (C2M2) and uses the ten domains from the C2M2 to inform the assessment process. The DER-CF extends the C2M2 to new pillars, domains, and controls appropriate for managing the security of DER and is appropriate for both existing DER as well as new projects to understand existing or potential risks. The domains in the DER-CF also include two that focus on issues related to supply chain risk management: External Dependency Management, which is part of the Governance Security Assessment and Systems/Device Management (including software integrity), which is part of the Technical Management Security Assessment.

External Dependency Management domain focuses first on identifying and prioritizing third parties and their role within the organization’s operations. This creates an understanding of the dependencies in the utility’s operations on third parties. These dependencies can then be mapped to the delivery of critical functions within the utility (e.g., that support the reliability and resilience of the electricity delivery). Ideally, the mapping will highlight where additional consideration is needed, such as finding additional suppliers.

With Systems/Device Management within the Technical Management vertical, the primary focus is on understanding the software and hardware supply chain. The assessment leads utilities through managing the risks of deploying third-party products and services, like counterfeit or compromised software, hardware, and services. 

As an outcome, DER-CF produces a prioritized list of recommendations based on the assessment results along with interactive dashboards for graphical representation of the organization’s cybersecurity posture.

## Cyber Informed Engineering
Cyber Informed Engineering returns the engineering side of operations to the consideration of the cybersecurity practices. This can be demonstrated by following a hypothetical cyber engineering problem and solutions at a Water Boost Station.

### CIE Water Pump Booster
Imagine a very small municipal water utility whose mission is reliably treating and distributing safe drinking water to all the citizens and businesses of the town. Water Booster Pumps generate and maintain pressure at the right levels to ensure water reaches every location in the service area. When changes are needed, operators travel by truck to booster stations to make the appropriate adjustments. The same manual approach is used when they need to gather operational information.

### The Call and The Opportunity
A cloud company called the water utility’s General Manager saying they could deliver remote monitoring and control of the pump boosters, saving time and money and freeing up operators for higher value tasks. The cloud company had security credentials; it was SOC2 certified, and its solution was developed using the secure development lifecycle.

### Considering the Offer
The water utility brought its engineers and cyber lead together as was the norm for big process changing decisions like this. An engineer asked how would the water utility know if someone accessed their equipment and made changes?  Would they have to wait to see the actual physical changes in pressure via their pressure gauges, customer complaints, or by other means? The answer was somewhere between “we don’t know, and we won’t know.”  

Another employee asked what’s the worst thing that could happen if a malicious attacker got access? The attacker could turn pump boosters off or on. Someone would have to go manually reset them, which would be annoying but not a catastrophe by any means. 

Finally, an engineer asked what if the attacker turned a booster on and off so rapidly it caused physical damage, basically destroying the pump? And what if they did this to all the pump boosters? Six months to fully recover, huge costs, and ability to deliver water uncertain—a true catastrophe.

### A CIE Solution
The group considered whether this risk was too much to bear and whether there could be any mitigation. One well-seasoned engineer suggested that a $20 time-delay relay—something he remembered played an important safety role back in the day—could do the trick. They could set the timer to allow only one change per 15 minutes or similar based on how long it takes the pump to shut down and for pressure transients to dissipate. A successful attacker would not be able to switch pumps off and on fast enough to damage them.

The only downside to this approach was that engineers would have the same limitation. They decided they could easily live with that, and in an extreme case, they could always suspend or ditch the cloud service and revert to the way they run their operations right now.

### Takeaways
They deployed an affirmative, last ditch security defense that’s under their complete control, which allows them to automate the right functions in ways that really help and make the operators jobs better. It’s not an EITHER/OR switch, it’s an AND. They get benefits of automation along with highest confidence security: A layered set of defenses.

### Introduction to Cyber-Informed Engineering (CIE)
Cyber-Informed Engineering (CIE) is the concept of integrating cybersecurity into the engineering design process to mitigate risks before they manifest. It emphasizes the importance of designing physical systems with inherent security to prevent cyber-attacks, rather than relying solely on traditional cybersecurity tactics like firewalls and antivirus software. CIE uses the insights of engineers and operators to design engineering controls which minimize the impacts of cyber-attacks.

### Application and Principles
CIE is applicable across various sectors, but the current work, funded by the U.S. Department of Energy, is particularly focused on the electricity sector. CIE is built around 12 principles, each with a key question that gets to the heart of the issue, as shown in Table 4. The first principle, Consequence-Focused Design, is critical to begin the CIE process. Utilities must understand their systems to develop solutions that extend engineering practices to address cybersecurity risks. Considering the impacts of cyber-attack as interruptions of desired functions highlights that cyber-attacks result in far more than the loss of data. They can impact operations, safety, and financial stability too.

Finally, CIE is a mode of working through the process of developing a robust security program. It complements many existing security best practices and standards like ISO/IEC 62443, the NIST Cybersecurity Framework, Process Hazard Analysis, and others. 

<table>
    <tr>
        <th>Principle</th>
        <th>Key Question</th>
    </tr>
    <tr>
        <td>Consequence-Focused Design</td>
        <td>How do I understand what critical functions my system must ensure and the undesired consequences it must prevent?</td>
    </tr>
    <tr>
        <td>Engineered Controls</td>
        <td>How do I implement controls to reduce avenues for attack or the damage which could result?</td>
    </tr>
    <tr>
        <td>Secure Information Architecture</td>
        <td>How do I prevent undesired manipulation of important data?</td>
    </tr>
    <tr>
        <td>Design Simplification</td>
        <td>How do I determine what features of my system are not absolutely necessary?</td>
    </tr>
    <tr>
        <td>Layered Defenses</td>
        <td>How do I create the best compilation of system defenses?</td>
    </tr>
    <tr>
        <td>Active Defense</td>
        <td>How do I proactively prepare to defend my system from any threat?</td>
    </tr>
    <tr>
        <td>Interdependency Evaluation</td>
        <td>How do I understand where my system can impact others or be impacted by others?</td>
    </tr>
    <tr>
        <td>Digital Asset Awareness</td>
        <td>How do I understand where digital assets are used, what functions they are capable of, and our assumptions about how they work?</td>
    </tr>
    <tr>
        <td>Cyber-Secure Supply Chain Controls</td>
        <td>How do I ensure my providers deliver the security we need?</td>
    </tr>
    <tr>
        <td>Planned Resilience</td>
        <td>How do I turn “what ifs” into “even ifs”?
        Engineering Information Control	How do I manage knowledge about my system? How do I keep it out of the wrong hands?</td>
    </tr>
    <tr>
        <td>Cybersecurity Culture</td>
        <td>How do I ensure that everyone performs their role aligned with our security goals?</td>
    </tr>
</table>


## Additional Resources
### DER-CF Resources:
* NREL’s [DER-CF](https://dercf.nrel.gov/)
* NREL, [Power System Cybersecurity Building Blocks](https://resilient-energy.org/cybersecurity-resilience)
* USAID/NREL/CARILEC [Cybersecurity Webinar Series](https://resilient-energy.org/cybersecurity-resilience/resources/webinars)
* NREL, [Gap Analysis of Supply Chain Cybersecurity for DERs](https://www.nrel.gov/docs/fy23osti/84752.pdf)
* NREL, [Supply Chain Cybersecurity Recommendations for Solar Photovoltaics](https://www.nrel.gov/docs/fy23osti/87135.pdf) 

### Cyber Informed Engineering Resources:
#### Websites
* [DOE CESER CIE Website](https://www.energy.gov/ceser/cyber-informed-engineering)
* [INL CIE Website](https://inl.gov/cie/)  
* [NREL CIE Website](https://www.nrel.gov/security-resilience/cyber-informed-engineering.html) 
#### Publications
* [CIE Implementation Guide](https://www.osti.gov/biblio/1995796) 
* [CIE Workbook for ADMS](https://www.osti.gov/biblio/1986517) 
* [CIE Workbook for Microgrids](https://www.osti.gov/biblio/2315001) 
* [CIE Workbook for Water Systems](https://www.osti.gov/biblio/2371031) 
* [CIE Assessment Tool](https://github.com/inlguy/CIE/releases/tag/v12.2.4.0) 
#### Articles and Briefings
* SANS [ICS Concepts Video](https://youtu.be/o_vIxW6UTeg)
* Industrial Cyber: [CIE and CCE Methodologies Can Deliver Engineered Industrial Systems for Holistic System Cybersecurity](https://industrialcyber.co/features/cie-and-cce-methodologies-can-deliver-engineered-industrial-systems-for-holistic-system-cybersecurity/) (June 11, 2023) with interviews from INL, 1898, and West Yost
* Harvard Business Review: [Engineering Cybersecurity into U.S. Critical Infrastructure](https://hbr.org/2023/04/engineering-cybersecurity-into-u-s-critical-infrastructure) (April 17, 2023) by Ginger Wright, Andrew Ohrt, and Andy Bochman

