---
title: "Conducting Cyber Risk Assessments"
weight: 23
# bookFlatSection: false
# bookToc: true
# bookHidden: false
# bookCollapseSection: false
# bookComments: false
# bookSearchExclude: false
---

# Conducting Cyber Risk Assessments for Supply Chain Risk Management

## Webinar
{{< youtube BC8pBz4AWis>}}

### Presenters
* **Frank Honkus**, E-ISAC
* **Mikhail Falkovich**, ConEd

## Summary
As supply chain operations become increasingly interconnected and digitalized, organizations must conduct cyber risk assessments on procured products and services and their suppliers. Supply chain risk management is a dynamic and ongoing process that requires an understanding of existing threats and vulnerabilities in all areas of the supply chain. Successful supply chain risk management tactics address prioritization, employ continual assessments, and involve collaboration with others up and down the supply chain and across the whole industry. Due to the breadth of supply chains, it is paramount that organizations stay vigilant in their own self-assessments and vendor evaluations.

Understanding vulnerabilities is a key component of understanding risk. Vulnerabilities exist in both the IT and OT space and can be found in hardware and software alike. Vulnerabilities in products introduce risk wherever they are deployed, both in terms of where on the network they are deployed or where, physically within the organization they are deployed. Vulnerabilities are not limited to products but may also exist in services as well, which can also introduce risk.

Country-of-origin risks represent one class of risks to consider. The country where products or services originate may not align with your organization’s security posture. That country’s standards of hardware and software development may not be sufficient. They may lack regulations to encourage secure development practices, or they may have regulations or local laws that actively require capabilities that could be concerning, like prioritizing the ability to monitor devices over privacy. There may also be concerns about using real-time support, which could result in connections from the country into your organization (e.g., for troubleshooting) or a phone call, which may be recorded and monitored.

As a hypothetical example, an electric utility may have a requirement in their procurement contracts that technology products should be manufactured within their own country, “Country X.” A product the utility procures may be assembled in Country X, but some of the internal hardware components were manufactured in “Country Y.” After deployment, the utility’s security team detects outbound communication between the product and the infrastructure of that foreign country, Country Y. 

In industry, it is common for manufacturers to source components from foreign countries and then assemble and resell the device in their home country. In this example, unbeknownst to the utility, the technology product used internal hardware components that were produced in Country Y. Supply chains can easily and unintentionally obfuscate some of these country-of-origin concerns.  


## Risk Mitigation Strategies

To address cybersecurity supply chain risks, organizations must manage these third-party risks. C-SCRM risks should be considered within the broader risk context, which could include potential financial, geopolitical, and cybersecurity risks introduced by any specific vendor. Organizations may choose to conduct a risk assessment of a vendor and their product internally or the organization may choose a separate vendor or aggregator to conduct the assessment. Regardless of choice of assessor, it is up to the purchasing organization to accept the risk. If the risk is deemed too high to accept, the purchasing organization will have to identify alternatives. Although there are standards and frameworks to help organizations assess risk, such as ISO 27001 and Service Organization Control 2 (SOC2), nothing is foolproof. Even the most well-functioning and well-protected third parties face the risks of cyberattacks and data breaches, so it is crucial that organizations take additional steps to mitigate and manage risk.

Another type of risk management strategy is the application of cybersecurity controls. Cybersecurity controls encompass a wide range of activities whose aim is to reduce risk. Risk assessments can help to prioritize and evaluate controls based on risk tier. The first step in a vendor product/service risk assessment is understanding the impact if that product fails or that service goes away. How much damage would that cause to business operations? The answer enables the organizations to assign that risk a tier, which they can use to identify the level of protection an asset requires. Not all failures are created equal; different levels of data sensitivity and operational significance require different levels of security. For example, a service that relies on the organization’s public data is much less risky in terms of data protection than a service that relies on proprietary company data.

The severity and impact of a risk can be unique to different organizations, so the organization must set thresholds and determine what is risky and what is less risky; nothing is risk-free. However, depending on the region and the industry, regulatory bodies may mandate compliance requirements for how to manage risk and validate controls (for example, North American Electric Reliability [NERC] Critical Infrastructure Protection [CIP] in North America). Organizations must ensure that their risk management strategies align with both their own internal needs and local regulatory requirements, if applicable. Assessing and ranking the cybersecurity risk of a third-party product or service drives both the application of security controls and the evaluation of vendors.

Organizations can align the criteria for vendor risk assessments to the risk tier associated with the potential use case. For vendors processing or accessing less sensitive data for relatively trivial tasks, self- certification (e.g., a signed document) attesting that the vendor has the requested cybersecurity controls in place, may suffice. That said, the purchasing organizations should reserve the right to audit. In cases where a vendor is accessing more confidential data or performing larger, more important tasks, the purchasing organization may find it more appropriate to delineate a set of functional criteria or have a third-party assessor evaluate the vendor to determine if the level of control is appropriate for the risk tier. Vendors accessing critical and proprietary data such as intellectual property face the highest level of scrutiny in evaluations such as full sets of detailed questionnaires and validating specifications and features with vendor architects and engineers.

The final risk management strategy prior to deployment is in the contractual terms and conditions.[^1]  The terms and conditions set the expectations for the business relationship. An example of this is defining the process and timeline of security notifications if the vendor has a security breach. Delays in notification from the vendor increase exposure and delay any internal processes to manage such security breaches.

{{% hint info %}}
**NATF Vendor Cybersecurity Questionnaire**
{.center}
Many utilities and organizations require vendors to respond to cybersecurity questionnaires and evaluations. Vendors may receive thousands of distinct questionnaires if every organization had its own evaluation process.
 
The North American Transmission Forum (NATF) managed a collaborative industry process to develop a Supply Chain Criteria and Risk Questionnaire, that is freely available, to manage this dilemma. The Risk Questionnaire was endorsed by NERC and has been implemented globally. Many vendors, in turn, have already completed this questionnaire, and maintain their responses to quickly provide this information to purchasing utilities.

![Screenshot of NATF Supply Chain questionnaire](figures/030_fig_callout.png)
Screenshot of the NATF Supply Chain Questionnaire
{.figure-caption}
{{% /hint %}}

## Risk Mitigations in Practice
Supply chain cybersecurity risk management is not only an external process to ensure that vendors implement and provide appropriate cyber risk mitigation tactics, but also an internal process as well. Mitigating risk is a company-wide effort requiring solution validation from all corners of an organization. From an architectural perspective, it is important to make sure that the appropriate architectures exist within the organization so that the product or service works as intended and is secured appropriately. From a privacy perspective, it is important to make sure that the correct datasets are included and protected. From a cybersecurity perspective, it is important to make sure that the required controls are both present in the product during procurement and fully functional and operational during deployment. 

Organizations typically employ Service Level Agreements (SLAs) in the procurement process; however, organizations must have their own internal mitigation measures in place in case a vendor does not meet the expectations defined in the SLA. Internal mitigation methods include architectural and process controls that mitigate risk and secure data, network segmentation to isolate and protect critical infrastructure, and active anomaly detection and monitoring to detect an incident before receiving a vendor security breach notification.

Furthermore, no vendor is perfect, and security events are always a concern. If the terms and conditions of an SLA have no consequences, the organization has no power or influence over the vendor, and the vendor has no impetus to improve performance. That said, building a trusted relationship with vendors can deliver benefits beyond following the minimum terms of the SLA. When organizations have a healthy relationship with vendors, there is a higher chance that the vendor is willing to collaborate and make requested changes to meet needs that lie outside of the SLA.

Supply chain cybersecurity risk management is a continuous process. Vendor assessments and evaluations must be continually performed and documented, such as evaluating their performance and level of support offered, among others. If a vendor or solution does not meet an organization’s needs, the organization needs to be able to pivot and identify alternatives.

## Additional Resources
* NATF [Documents](https://natf.net/documents)
* NATF [Energy Sector Supply Chain Risk Questionnaire](https://www.natf.net/docs/natfnetlibraries/documents/resources/supply-chain/energy-sector-supply-chain-risk-questionnaire.xlsx) (xlsx)
* NATF [Supply Chain Risk Management Guidance](https://www.natf.net/docs/natfnetlibraries/documents/resources/supply-chain/natf-supply-chain-risk-management-guidance.pdf) (pdf)
* NATF [Supply Chain Security Criteria](https://www.natf.net/docs/natfnetlibraries/documents/resources/supply-chain/natf-supply-chain-security-criteria.xlsx) (xlsx)
* EEI, [Model Procurement Contract Language Addressing Cybersecurity Supply Chain Risk](https://www.eei.org/-/media/Project/EEI/Documents/Issues-and-Policy/Model--Procurement-Contract.pdf), Version 3.0, October 2022


[^1]: See for example, Edison Electric Institute (EEI) Model Procurement Contract Language Addressing Cybersecurity Supply Chain Risk. Version 3.0 (October 2022)