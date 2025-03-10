---
title: "Cybersecurity Incident Response Plan Development"
weight: 41
# bookFlatSection: false
# bookToc: true
# bookHidden: false
# bookCollapseSection: false
# bookComments: false
# bookSearchExclude: false
---

# Cybersecurity Incident Response Plan Development

## Webinar
{{< youtube ve8xidjns0w >}}

### Presenters
* **Michael Martin**, Chelan County PUD
* **Tony Assan**, GRIDCo (Ghana)

{{% hint warning %}}
“The goal of an incident response plan is to establish a written systematic approach” 

---Michael Martin, Chelan County PUD
{.right}
{{% /hint %}}

{{% hint warning %}}
“Supply chain has become one of the most challenging vulnerabilities to address”
 
---Tony Assan, GRIDCo
{.right}
{{% /hint %}}

## Summary
Incident response planning is an essential control for electric utilities given the digitalization of OT systems. Developing an incident response plan is the first control in the SANS Institute’s “The Five ICS Cybersecurity Critical Controls,” in part because it can help utilities determine what additional controls can deliver the highest value. That is, additional cybersecurity controls should support the capabilities the utility needs to have an effective incident response. 

Two case studies below discuss two utilities’ approaches to developing incident response plans: Chelan County Public Utility District (Chelan PUD), a generation/transmission/distribution utility in the United States and GRIDCo, the electric transmission grid operator in Ghana.

## Case Study: Chelan County Public Utility District

Chelan PUD operates in the northwest United States, managing three hydroelectric dams. These facilities produce a significant amount of electricity (totaling roughly 7.5 million MWh in 2023), and they sell surplus electricity to neighboring utilities. Chelan PUD also provides transmission and distribution services with more than 3,000 km of distribution lines. This backdrop underscores the critical need for a robust cybersecurity posture to protect the utility’s OT, as an operational impact could affect many customers and businesses.

### Adopting the NIST Cybersecurity Framework
Chelan County PUD began overhauling their incident response plan in 2016 to comply with NERC CIP regulations. This effort was informed by key documents like the NIST Special Publication 800-61 Revision 2, “Computer Security Incident Handling Guide” and the Department of Homeland Security's guide on “Developing an Industrial Control Systems Cyber Security Incident Response Capability.” The adoption of the NIST Model was pivotal in this strategic redirection. The NIST Model highlights four interconnected phases: Preparation; Detection and Analysis; Containment, Eradication, & Recovery; and Post-incident Activity, as shown in Figure 12.

![Four-step process to developing incident response capabilities.](/images/060_incident_response_process.png)  
Figure 12. Four-step process to developing incident response capabilities.
{.figure-caption}

### Preparation: Identifying Critical Utility Assets
The preparation phase involved applying NERC CIP classification criteria to identify critical assets and applying physical and cybersecurity controls based on their impact assessment. NERC CIP regulations require identifying and classifying critical cyber assets and their supporting systems with either high, medium, low, or no impact to the greater interconnected power grid. Based on these impact ratings, these systems are then protected by appropriate physical and cybersecurity controls to mitigate their associated risks. Chelan PUD conducts business impact risk assessments to identify additional mitigations like insurance, support agreements, and preventative maintenance to enhance resilience.

### Writing Your Incident Response Plan
When developing an incident response plan, the best approach is to get something put on paper. The first draft does not have to be perfect, and a “Crawl, Walk, Run” approach to maturing the plan is effective. That is, utilities should create a basic plan first and improve it over time to the point where it becomes fully fleshed out and functional for all parties involved. Once you have a plan, implementing lessons learned from incident response plan exercises is the most effective method to improve your plan. Chelan PUD’s IT department used the American Public Power Association’s Public Power Cyber Incident Response Playbook (2019) as a guide to developing their cyber incident response plan. 

![Example cyber incident handling process flowchart](/images/060_Example_Incident_Response_Flowchart.png)  
Figure 13. Example cyber incident handling process flowchart (Source: APPA 2019 via Michael Martin)
{.figure-caption}

### Cybersecurity Incident Response Plan: Key Elements
A successful Cybersecurity Incident Response Plan should include the following key elements:
* **Roles and Responsibilities:** Clearly defining the roles of all participants in the response process
* **Detection:** Distinguishing incidents from normal events
* **Containment:** Actions to take to prevent further damage
* **Eradication:** Removing the threat
* **Recovery:** Steps to restore the system to full operation
* **Communication Plans:** Documenting communication methods and how communication occurs between departments and to external groups

NERC defines a cybersecurity incident as: “A malicious act or suspicious event that … disrupts or attempts to disrupt the operation of a utility cyber system.” To detect a cybersecurity incident, it is important to train system operators and system administrators on what to look for. The NERC “Cyber Intrusion Guide for System Operators” and the NIST SP 800-82 Revision 3, “Guide to Operational Technology Security” documents list possible incident indicators specific to typical roles and responsibilities. A decision tree or flow chart (see Figure 14) can be helpful. As part of the “detection” capability, utilities should document methods to report suspicious activity as well as procedures to analyze potential incidents and preserve evidence for later review.

Containment and eradication require the utility to act swiftly, so playbooks for likely scenarios can be very useful. Incident response plans should briefly list common incident types (like malware, ransomware, account misuse) and their potential containment actions since these may be overlooked during an incident. An excellent playbook for ransomware is the U.S. Cybersecurity and Infrastructure Security Agency’s (CISA’s) “Stop Ransomware Guide.” References to playbooks like this can be an excellent starting point or reference for an incident response plan.

Recovery may be an extended process and will highlight many opportunities for future improvements. Utilities should document all the steps necessary to restore the system back to full operation. Some essential strategies for recovery include keeping spare hardware for human-machine interfaces (HMIs), computers, PLCs, remote terminal units (RTUs), and network switches in case of supply chain delays. Equipment like this can have a long lead time—for example, Chelan’s preferred network switch had a 180-day lead time—so spare inventory may be essential.

![Example decision tree from Chelan PUD's incident response plan.](/images/060_Example_Decision_Tree.png)  
Figure 14. Example decision tree from Chelan PUD's incident response plan. (Source: Michael Martin, Chelan PUD)
{.figure-caption}

Communication plans are often overlooked. Communication methods between coworkers is the most important aspect of incident response recovery. Everyone should know the preferred communication method such as cell phones, Slack, Teams, WhatsApp, Zoom. In addition to having a preferred method, include backup options in case one system is down, including a manual method of communication if there is no telecommunication method available. It is also important how information will be relayed from one response team to another, so that there is a clear point of contact and task delegation system in place. Lastly, in addition to internal communication plans, utilities should include a way to contact external groups such as law enforcement, neighboring utilities, and the general public.

### Exercise Your Incident Response Plan

Regular practice through tabletop drills and simulation of recent scenarios is crucial for identifying plan strengths and areas for improvement. Annual exercises are recommended, focusing on real-world scenarios to enhance response readiness. A good way to simulate exercises is to test recent scenarios that occurred in the news to other utilities or organizations. The SolarWinds attack is an excellent example of a supply chain attack that utilities can adapt to their own situations. The Ukraine grid attacks and/or Colonial Pipeline attack as well as an insider threat scenario are also good examples to build from. To improve your plan, ensure that all members of the response teams actually use the plan during the exercise.

After the exercise, conduct a lessons-learned meeting to gather feedback to refine the incident response plan. This process helps identify performance gaps, informational needs, and potential improvements for future response efforts. These exercises are excellent ways to offer training opportunities for responders so that during an actual event, confusion is minimized. For example, Chelan found that their plan was too long, so they made it shorter and more actionable with decision trees and checklists. Similarly, by having the response team stay at their desks rather than gather in a conference room to test their plan, Chelan discovered several new communications challenges not reflected in their communication plan.

Finally, these exercises highlighted ways to improve the utility’s cybersecurity and physical security posture. These included application architecture improvements, additional security cameras, penetration tests for specific networks, enhanced event notification (e.g., after-hours alerts), and additional tools deployed (e.g., network monitoring solutions to support operational troubleshooting and forensic analysis).

## Case Study: Ghana GRIDCo

GRIDCo operates Ghana’s transmission system, servicing 32 bulk customers and 10 generating companies, including independent power producers, with a significant installed generation capacity from hydro, thermal, and solar plans as well as more than 6,000 km of transmission infrastructure. GRIDCo separates IT and OT infrastructures, emphasizing the importance of robust cybersecurity practices to mitigate the potential financial and operational impacts of outages. GRIDCo’s transmission infrastructure is interconnected with neighboring countries, Côte D’Ivoire, Burkina Faso, Togo, and Benin, which significantly extends the potential impact of an outage, including financial losses in the millions of US dollars per day, impacts to national gross domestic product (GDP), and sub-regional security and stability.

### OT Security and Incident Management Considerations

GRIDCo identified a compelling basis for developing an incident response plan for OT, with additional focus on the supply chain for OT. First, they recognized that threat actors could target any part of an OT system’s lifecycle. Second, attackers have been increasingly targeting industrial control systems and third parties to carry out attacks. Finally, GRIDCo needed to understand their suppliers’ maturity and security processes for connected products and services to have assurance that these practices aligned with their own expectations. 

GRIDCo also approached security differently for their OT and IT systems, noting key differences between the two. OT systems, which directly control devices and processes, require unique considerations for incident response due to their specialized place within operations, long refresh cycles, and high exposure to zero-day vulnerabilities. In contrast, IT systems, focused on information management and security, generally have shorter refresh cycles and better-defined paths for threat identification and remediation. Solutions that work in the IT environment can be detrimental in the OT environment; equipment on the OT side, especially older equipment, have failed when scanned by security solutions designed for IT networks. Developing incident response plans unique to IT and OT may be essential.

### GRIDCo's OT Incident Management Plan
Adhering to the NIST Guide to OT Security (800-82 Rev. 3), GRIDCo developed a comprehensive Incident Management Plan (IMP) that spans the four main phases shown in Figure 12.

#### Preparation and Prevention
GRIDCo prioritizes the identification and protection of critical systems, employing a business impact analysis to inform their cybersecurity posture. They have adopted a key performance indicator (KPI) that they must be able to restore 80% of operations within 48 hours of an outage. Their incident response plan is specifically designed to achieve this with 95% certainty.

The business impact analysis is driven by their existing risk analysis processes. This process relies on multiple teams from finance, procurement, and engineering to determine the probability of an incident and the potential impact of the incident. They draw on their experience as well as contract terms to estimate the probability. Similarly, GRIDCo uses financial analysis to estimate potential impacts to then calculate risk and business impact. 

GRIDCo then compares the results of the business impact and risk analysis with the treatment costs (i.e., the costs to implement controls to address the risk), as well as any residual or remaining risk. In the end, GRIDCo has confidence that they have appropriately matched their controls with their risks.

#### Detection and Analysis
Because supply chains can have a large impact on their cybersecurity posture, GRIDCo emphasizes vetting and collaborating with vendors to ensure cybersecurity compliance from the design phase through implementation. Vendors must demonstrate that they meet GRIDCo’s criteria to participate in the tender process. In addition, GRIDCo considers security in the design phase, so that security requirements are embedded within the product. They inspect and validate the vendor’s documentation and claims, even going so far as to require factory acceptance testing (FAT). Similarly, GRIDCo tests cybersecurity functionality (e.g., validates firewall rules) as part of a Site Acceptance Test (SAT) during deployment. Because people are key to security, GRIDCo also reviews whether the vendor has a culture of security to understand whether the vendor is likely to be responsive if there is an incident.

#### Containment, Eradication, and Recovery
GRIDCo has not had a service interruption but has had incidents that required response. In the past, their detection created many false positives, which they have worked to reduce through iterative improvements, such as deploying new triage processes and new systems to help identify false positives. Fewer alerts mean GRIDCo can act on the alerts that do arise. Upon detection of an issue, GRIDCo quickly initiates a well-structured response process (see Figure 15), focusing on rapid containment and recovery to minimize operational disruptions. Their incident management process includes communication internally as well as with three external groups that GRIDCo is required to inform according to local regulations. 

![GRIDCo's response process from incident logging to resolution and closure.](/images/060_Incident_Response_Process_from_logging_to_resolution.png)  
Figure 15. GRIDCo's response process from incident logging to resolution and closure.
{.figure-caption}

#### Post-Incident Activity
Regular testing and simulations drive continuous improvement of the incident response plan, with lessons learned integrated into future iterations. These simulations are as realistic as possible. GRIDCo maintains a log of all lessons learned and reviews their plan at least annually.

Recognizing the supply chain as a critical vulnerability, GRIDCo implemented measures to assess and manage the cybersecurity risks associated with suppliers and third parties. This includes maintaining a categorized database of suppliers for periodic cybersecurity compliance assessments and pre-tender cybersecurity evaluations.

{{% hint info %}}
**Procurement Example: GRIDCo’s SCADA Upgrade**
{.center}

GRIDCo applied the process when they upgraded their SCADA system and deployed a new disaster recovery site control center in 2023 through several key actions: 
* Including security considerations during the scoping and requirements gathering phase, before seeking vendors, to ensure security-by-design.
* Pre-qualifying prospective vendors to ensure any vendor selected would meet their security requirements. Moreover, the tenderers had to accept responsibility for undeclared vulnerabilities.
* Traveling to Europe to evaluate vendors practices and their products at the source. Outstanding issues were documented to ensure that they were resolved before taking delivery.
* Conducting SATs including cybersecurity reviews (e.g., firewall configuration audits, hardware and operating system hardening, Active Directory configuration, and redundancy assurance).
* Finally, they conducted a red-team attack to demonstrate that the system operated as expected. 
{{% /hint %}}
 
## Cybersecurity Incident Response Plan Suggestions
* Make available response plans and related information in print and on intranet (contact list, vendor information)
* Put the plan revision date in a header/footer on each page to identify the current version
* Establish delegates or backups for each role, so incident response isn't slowed when someone is not available
* Empower relevant people to make decisions to facilitate efficient response
* Document incident response resources in your plan (contracted incident response service, government resources, insurance, etc.)
* Through Cybersecurity Awareness programs, make all users aware of the company’s Incident Response protocols, including how to initiate them
* Include possible simulations in the plan to test the plan periodically to ensure effective compliance

## Additional Resources
* American Public Power Association, [Public Power Cyber Incident Response Playbook](https://www.publicpower.org/system/files/documents/Public-Power-Cyber-Incident-Response-Playbook.pdf) (2019) 
* NIST SP 800-61 Revision 2, [Computer Security Incident Handling Guide](https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-61r2.pdf) (2012)
* NIST SP 800-82 Revision 3, [Guide to Operational Technology (OT) Security](https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-82r3.pdf) (2023)
* NIST SP 800-83 Revision 1, [Guide to Malware Incident Prevention and Handling for Desktops and Laptops](https://nvlpubs.nist.gov/nistpubs/specialpublications/nist.sp.800-83r1.pdf) (2013)
* NERC [Cyber Intrusion Guide for System Operators](https://www.nerc.com/comm/RSTC_Reliability_Guidelines/Reliability_Guideline-Cyber_Intrusion_Guide_for_System_Operators.pdf) (2023)
* CISA [#StopRansomware Guide](https://www.cisa.gov/sites/default/files/2023-10/StopRansomware-Guide-508C-v3_1.pdf) (2023)
