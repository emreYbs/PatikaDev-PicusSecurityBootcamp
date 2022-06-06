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

- 

- 
- 
- 

## Possible Issues

- "Problem:staff shortage"
High staffing requirements.Do our capabilities match our business-needs with our current staff?  Staff in SOC work overtime and this can tire them. So we need to  check SOC staffing levels in comparison to our business growth over time, and invest/train new staff when needed. Also some work can be bypassed to outsourcing. Outsourcing can be useful to overcome some of the issues that SOC users face. You can gain expert help and also by letting some of the work to oursourcing parties, it is possible to decrease the burden on our staff. Outsourcing can also be cost effective. To sum up, we need to ask this question to ourselves: "Does staffing match our growth?". If we need more staff, we need to find the talented ones or train and make them ready or oursource some work. So we can also help our other staff to feel less tired. Tp remediate the staff shortage problem, companies can organize Bootcamps and co-operate with the relevant departments in the universities. 



- "Problem: Lack of skilled staff and knowledge shortage". Finding and retaining talented staff is another issue like the staff shortage that I mentioned above. In this case you can find staff but they are not job ready and there is no real entry job in cybersecurity. Even an enrty level applicant has to have some experience and training to work in entry positions. So talented staff is really needed and it is not easy to find and retain them.Moreover, frequent turnover appears to be another obstacle if we can find the talented staff, because they may quit for various reasons like pay rise offer from a rival company.The average duration of employment is predominantly less than five years according to a recent SANS report I have read. Talent pool is still not adequate and finding and also retaining skillful staff is a major problem. Also if a talent is given inadequate salary, then he/she may quit and it can be difficult to find a replacement. Teams in SOC must regularly rank cybersecurity threats in terms of potential damage so they need to have the wide knowledge on various areas of cybersecurity. If they have the knowledge and the required experience, then they can prioritize the tasks in SOC. Moreover, only talented and experienced SOC teams can rapidly identify and remediate attacks to minimize the impact of cyber threats on the companies. If your response to a cyber attack is too slow, then, the impact of the cyber attack is more destructive and bad for your reputation as well.


- "Problem: Alert Fatigue". Too many alerts are generated by our SIEM, EDR tools and also nearly half of them are false possitives. So our SIEM users can’t look into all of them and also the lack of correlation among alerts can cause tiredness among our SOC staff/users. We need to combat alert fatigue to accelerate threat detection and response capabilities of our Security Operations Center. Moreover, we should reduce the burden on our staff caused by alert fatigue of SIEM tools.Their attention can be negatively affected by too many alerts when they do not provide real value and context. In short, we can validate the alert rules in our SIEM/EDR and identify detection gaps with the detection analytics feature of SIEMs. The Picus Security Control Validation Platform has these capabilities because after watching Purple Academy Training videos, I also used the 14 days trial and examined the capabilities and liked the contextual alert rules which can overcome the issue of the possible detection gaps. Furthermore, the video explained the need for a transaction form a reactive SOC to proactive SOC because proactive SOC provide contextual and necessary logs. So it mitigates the alert fatigue and this helps our SOC team and their performance. If we can find a proper solution to alert fatigue and decrease the number of false or positive alarms, we can also decrease the process latency.



 _(Since we are asked to write 5 at most, I will try to blend some related issues and do my best to integrate and show their connection as a whole. Otherwise, I needed to write/reply 6-7 issues:)   [Please write at most five prioritized issues]_
 
- "Problem: Technology" Technology also creates challenges for SOC teams. Lack of adequate tooling, lack of automation and integration, inadequate analytics and filtering, lack of enterprisewide visibility and lack of proper log management in a contextual way". 
This can also lead to serious problems which we obviously do not want. Lack of context can result in omitting some possible serious findings in our logs. Humans need a context to understand in a more efficient and meaningful way.
For possible solutions, automation and orchestration and tools' integration is needed. Too many tools that are not integrated is a problem and automation and orchestration can help to overcome this issue if we have skillful/trained staff. In short, metrics are a critical component of the SOC’s interaction with the organization. Yet, most of the metrics used fail to effectively characterize the value the SOC provides to the business. Therefore, we need to increase the enterprisewide visibility by proper metrics. We live in a data-driven worl in a way and the future will be based on data science. So, we need to have the right metrics and validate these metrics as well. Our metrics can also give us the answers of these questions:"Is our technology working? What’s effective?, What is ineffective".
Prior to establishing a SOC, an organization must define its cybersecurity strategy to align with current business goals and problems. That is why we need enterprisewide visibility and validate our metrics.

My answer to this question "What are the possible results and changes in the organization using the solution?" is:

By the help of the needed tools, proper metrics and validation of our metrics we can have a better assessment of the trends in cybersecurity, current cyber threats, provide better service to our users/customers and a have better share in the market. So we need to ask ourselves "Do we use the necessary tools properly?", "Are Trends in technology/cybersecurity going in the right direction?"
If we do not have proper tech stack to cope with logs, proper log management, proper threat intelliegence and enterprisewide visibility, then we will end up in business blindness which will cause many issues for us. For example, if we blindly follow trends in cybersecurity and trust 100%, then we may tend to follow a possible wrong path. We need to access the effectiveness and success of various trends. We can define and track the critical metrics to our organization and thus we can ensure that our organization are going in the right direction.


- Lack of budgeting. A realistic model of required investment should be developed and necessary investment should be provided. Besides, management and SOC leads/managers
work together closely to decide how to allocate funds for cybersecurity. From the reports I have read, I can say that management tend to take recommendations
from SOC leads/managers but frequently goes against SOC management’s recommendations. Thus this can be a issue because this can de-motivate the SOC team and users of SOC can be adversely affected as a result. In short, we need to make sure our organizational management listens to SOC users' feedbacks, suggestions so the budget is not allocated on the wrong basis. We should focus on mitigating the threats with the greatest potential for damage so budget planning has to be flexible according to necessity. To effectively protect the enterprise, SOC teams need tools that enable them to maximize the effectiveness of their limited teams and resources. Hence, budget planning should take this into account.








