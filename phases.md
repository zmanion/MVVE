<img width="992" height="375" alt="image" src="https://github.com/user-attachments/assets/16dcfd45-ebfb-43c1-bb95-5de465a3ab4a" />

## Phase 0: Introduction of Vulnerability
Vulnerability is introduced into a product during development, either through direct coding, third-party dependency or indirect dependencies and remains latent through deployment.

## Phase 1: Initial Discovery of Vulnerability
Latent vulnerability is discovered by either an internal actor (developer, red team, security tool) or external actor (independent researcher, bug bounty participant, penetration tester, etc), or by adversarial exploitation or other disclosure of the vulnerability.

## Phase 2: Private Coordination
The research (party who initiated phase 1) and product producers may collaborate to confirm scope, verify exploitability, share PoCs, discuss mitigations and set timelines. This phase is unfortunately and incorrectly treated as optional by some external parties.
This phase may expand in scope to coordinate with vulnerability scanners to provide defender with day 0 discovery signatures. 
Producer could discover in 1, 2, 4, or 5, in 4 or 5 is a risk-increasing race, so CVD prefers 1 or 2

## Phase 3: Public Disclosure
The vulnerability is disclosed via vulnerability databases (CVE), vendor advisories and other notification methods, could also be triggered by discovery of exploitation of the vulnerability in the wild. 

## Phase 4: Information Published to Vulnerability Enumeration
Information elements for vulnerability are published to vulnerability enumeration, preferably with the minimally viable information elements (MVVE) defined below.

## Phase 5: Public Discovery/Notification
The product consumer and/or vulnerability manager discovers (is notified of) the existence of the vulnerability, but may not be aware of any local instances of specific vulnerable products. Enough information should be provided to enable product consumers and/or vulnerability managers to progress through the rest of the vulnerability lifecycle phases. 

## Phase 6: Discovery of Vulnerable Instances
Product consumers/vulnerability managers must have enough information to discover/determine if one or more products in their environment are affected by the vulnerability. Information elements from Phase 4 must minimally contain enough information to support the product consumer/vulnerability manager to this point of discovery. 

## Phase 7: Local Analysis and Enrichment: Pre-Prioritization
Environmental information and any contextual information that may enable more accurate prioritization in the following phase. Information such as software settings and configuration(s) that may enable or prevent exploitation, network connectivity and reachability analysis informing general exposure, perhaps other specific information such as asset importance and adjacency may support and improve the prioritization phase. It may also be beneficial to understand existing security controls and their strengths and limitations and how they would apply to local instances of vulnerabilities. Note that some information discovered in this phase may make real world exploitation impossible at the current point in time, but that does not negate the presence of vulnerable products.
Collecting information useful/necessary for 8

## Phase 8: Prioritization (of Remediation tasks)
With over 40K+ new CVE Records per year and the average windows platform hosting more than 100 open vulnerabilities a month. prioritization becomes essential as the number of identified vulnerabilities can rise into the hundreds of thousands or even millions. If remediation procedures didn’t require rigorous testing and product producers supplied easy to apply patches, prioritization may be much less important. But in our current environment, prioritization is not just important, it’s a fact of operating a business and accurate and efficient prioritization requires good risk assessment practices. For the purpose of our discussion here, prioritization is both enabled and ultimately improved with better and more accurate information not just about the vulnerability (product consumers and vulnerability managers will turn to vulnerability enumerations and enrichment sources),  but also about the local context, asset and network information to support their vulnerability prioritization.

## Phase 9: Remediation Communication and Coordination
Often the vulnerability manager or product consumer must coordinate with administrators or other technology professionals, whether through formal ticketing systems or informal discussions with everything in between. In less complex environments this phase may not exist, while in more complex environments the communication and coordination requires concerted effort to maintain. 

## Phase 10: Remediation Tasks
Prioritization guides Remediation: actions performed by the vulnerability manager to respond to the (risk posed by the) vulnerability. Commonly, perhaps ideally, remediation means updating, upgrading, or patching software to explicitly remove the vulnerability. There are many other possible Remediation actions, including external compensating controls and risk assessment (i.e., intentionally taking no Remediation action).
In a typical “scan, patch, repeat” cycle, successful Remediation is tested by a future scanning or vulnerability detection run. The accuracy of vulnerability detection is important and seems to suffer broadly from false positive rates, but that is not something we address here.
 
## Phase 11: Reporting and Monitoring
Monitor, collect feedback, and periodically analyze and adjust (improve) the vulnerability management process
 
## Phase X: Everything Else
Tasks outside of the lifecycle that support or inform the other tasks. Not necessarily the last phase as these tasks can and do occur earlier in and throughout the lifecycle, but they are not explicitly required in the lifecycle. For example, Intel related tasks such as generating signatures to detect/prevent exploitation, sharing IoCs and monitoring for exploit variants. Opportunities for developer training/awareness, vulnerability vendor products, and data-driven vulnerability research seeking to advance our state of knowledge.
Threat, threat intel (exploit detection, ITW/KEV, incident reporting)

