# Challenges encountered to operationalize EDRs.

- First of all, there is a lack of human resources. According to a SANSsurvey, security incident response teams of 77% of organizations are comprised of only five members or fewer.
- Moreover, it is hard to use any EDR. According to CyberProof, it takes more than 6 months to build a baseline to start using an EDR properly.
- The last one is a well-known challenge by EDR users.Half of all alerts given by EDR are false-positives,  according to the Ponemon Institute,

These challenges lead directly to my next point. 
### An EDR is no silver bullet,
and there are some major problems security teams need to overcome in using EDRs.

- First of all, EDR is not a plug-and-play solution. Aligning default EDR policies to organizational needs and building an adequate rule-base takes time. Defining the scope of telemetry, deciding what threats to detect first, identifying what assets to protect first are challenging. 

- After creating a rule base, keeping EDR configurations up-to-date against new attack techniques is not so straightforward. You have to set the right priorities. Not every attack may be relevant or pose a high-risk. Overpopulating EDRs with detection rules can create a flood of low-priority alerts, false positives, and as a result, alert fatigue. The number of alerts may go over organizational capacities, and process load may delay alert generation. 

- On the flip side, not having enough detection rules will result in gaps. Avoiding alerts may mean missing some critical events. Security teams do need to strike a fine balance here.

- Moreover, changes on endpoints, such as operating system and application updates, new and retired applications, and access policies impact the efficacy of the existing detection policies.





# Solutions ( oku ve ödevde özetle)

Planning


### The first stage is Planning.
In this stage, you can identify the detection gaps in your EDR by using the detection analytics function of a comprehensive BAS solution.
How can you prioritize detection gaps in EDRs? 

- BAS solutions map simulated threats to the MITRE ATT&CK framework. Simulate threats, map the created alerts to the ATT&CK techniques, and identify your weakest techniques. So, you can shortlist MITRE ATT&CK techniques that have the lowest detection rates.
- 
- It is also a quick win to start with logged but not alerted attacks. Simulate the threats shortlisted in the gap analysis, identify threats that we have logs but no alerts. If you have required logs for a TTP, it will be more straightforward to write alert rules for this threat. 




Development

### The second phase is Development, which includes the Design, Implementation, and Test & Validate phases.

- Firstly, you should identify the logs to have the required data visibility for threats.

- Then, you can start implementing the rules. 
 -- As a quick win, you can identify built-in but not activated rules by the vendor of the EDR.
 -- You can also utilize third-party rule libraries. For example, Picus Mitigation Library includes more than 1,000 detection rules with the relevant detailed thread information. It decreases your time-to-response, especially in outbreaks.
 -- As another option, you can develop your own rules if you have the required resources. 

- Testing and validating rules are also important to find whether the rule can detect the intended threat and whether it gives false positive or false negative results.
 -- You can use peer or third-party reviews to validate your analytics. Of course, you can automate this test and validation face by using the Detection Analytics function of a comprehensive BAS solution.
 -- In addition to determining false positives and false negatives, it is important to determine performance problems.
 
 
 Breach and Attack Simulation (BAS) platforms, can help solving these problems. Picus Security has an efficient Breach and Attack Simulation platform. The Picus BAS is an end-to-end Security Control Validation Platform. Picus provides a rich threat context for cyber defense teams by giving actionable Threat Intelligence. Threats and threat groups are merging and different actor vectors occur. So updated threat intelligence is a must for an attack breach attack simulation.
 So, identifing problems and also giving actionable insights via these threat intelligence will be more efficient.
 
 Actionable alert rules and required log sources enable fast response to the detection gaps in user's environment.
 
 
 You can validate the alert rules in your EDR and identify detection gaps with the detection analytics feature of the Picus Security Control Validation Platform.
 
 
 
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------

# Questions to ask/consider:

- Are Trends Going in the Right Direction? AI can be over-emphasized or blindly trusted. If we blindly follow trends in cybersecurity and trust 100%, then we may tend to follow a possible wrong path. We need to access the effectiveness and success of various trends. We can define and track the critical metrics to our organization and thus we can ensure that our organization are going in the right direction.

- Does staffing match growth?
- Do capabilities match business need? Prior to establishing a SOC, an organization must define its cybersecurity strategy to align with current business goals and problems.
- Is the technology working? what’s effective?

## Possible Issues

- High staffing requirements. Staff in SOC work overtime and this can tire them. So we need to  check SOC staffing levels in comparison to our business growth over time, and invest/train new staff when needed. Also some work can be bypassed to outsourcing.
- Lack of skilled staff and retaining talented staff is an issue. Frequent turnover appears to be the first
- obstacle.The average duration of employment is predominantly less than five years according to a recent SANS report I have read.
- Too many alerts that we can’t look into (lack of correlation between alerts)
- Too many tools that are not integrated
- Lack of automation and orchestration
- Lack of enterprisewide visibility
- Lack of context 
- Lack of budgeting. A realistic model of required investment should be developed and necessary investment should be provided. Besides, management and SOC leads/managers
work together closely to decide how to allocate funds for cybersecurity. From the reports I have read, I can say that management tend to take recommendations
from SOC leads/managers but frequently goes against SOC management’s recommendations. Thus this can be a issue because this can de-motivate the SOC team and users of SOC can be adversely affected as a result. In short, we need to make sure our organizational management listens to SOC users' feedbacks, suggestions.

- Metrics are a critical component of the SOC’s interaction with the organization. Yet, most of the metrics used fail to effectively characterize the value the SOC provides to the business.
- Outsourcing can be useful to overcome some of the issues that SOC users face. You can gain expert help and also by letting some of the work to oursourcing parties, it is possible to decrease the burden on our staff. Outsourcing can also be cost effective.



