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
 -- You can also utilize third-party rule libraries. For example, Picus Mitigation Library includes more than 1,000 detection rules with the relevant detailed threat information. It decreases your time-to-response, especially in outbreaks.
 -- As another option, you can develop your own rules if you have the required resources. 

- Testing and validating rules are also important to find whether the rule can detect the intended threat and whether it gives false positive or false negative results.
 -- You can use peer or third-party reviews to validate your analytics. Of course, you can automate this test and validation face by using the Detection Analytics function of a comprehensive BAS solution.
 -- In addition to determining false positives and false negatives, it is important to determine performance problems.
 
 
 Breach and Attack Simulation (BAS) platforms, can help solving these problems. Picus Security has an efficient Breach and Attack Simulation platform. The Picus BAS is an end-to-end Security Control Validation Platform. Picus provides a rich threat context for cyber defense teams by giving actionable Threat Intelligence. Threats and threat groups are merging and different actor vectors occur. So updated threat intelligence is a must for an attack breach attack simulation.
 So, identifing problems and also giving actionable insights via these threat intelligence will be more efficient.
 
 Actionable alert rules and required log sources enable fast response to the detection gaps in user's environment
 
 
 You can validate the alert rules in your EDR and identify detection gaps with the detection analytics feature of the Picus Security Control Validation Platform.
 
 
 
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------


## Possible Issues


- "Problem:Staff shortage, high staffing requirements."
There is a lack of human resources. According to a SANSsurvey, security incident response teams of 77% of organizations are comprised of only five members or fewer.
Technology is rapidly evolving and especially after Covid19 pandemic and remote work necessities, cybersecurity threats has increased. Threat actors are more talented and they have financial support. Some of the advanced threat actors are supported by some countries, intelligence agencies and mafia. Also cloud computing is very popular and it seems it will be much more common in the following years. However, there is a staff shortage in cybersecurity. There are not enough stuff, especially talented and job ready ones. Another issue is that companies try to expand, however, most of them are under-staff. So, we need to ask ourselves "Do our capabilities match our business-needs with our current staff?"

Staff in SOC work overtime and this can tire them. So we need to  check SOC staffing levels in comparison to our business growth over time, and invest/train new staff when needed. Also some work can be bypassed to outsourcing. Outsourcing can be useful to overcome some of the issues that SOC users face. You can gain expert help and also by letting some of the work to outsourcing parties, it is possible to decrease the burden on our staff. Outsourcing can also be cost effective. To sum up, we need to ask this question to ourselves: "Does staffing match our growth?". If we need more staff, we need to find the talented ones or train and make them ready or outsource some work. So we can also help our other staff to feel less tired. To remediate the staff shortage problem, companies can organize Boot-camps and co-operate with the relevant departments in the universities.

..................................................................

- "Problem: Lack of skilled staff and knowledge shortage". The cybersecurity industry is experiencing a significant skills gap. This makes it difficult for organizations to attract and retain the talent required to protect themselves against cyber threats. Finding and retaining talented staff is another issue like the staff shortage that I mentioned above.  In this case you can find staff but they are not job ready and there is no real entry job in cybersecurity. Even an entry level applicant has to have some experience and training to work in entry positions. Moreover, it is hard to use any EDR, next generalization firewalls, etc. According to CyberProof, it takes more than 6 months to build a baseline to start using an EDR properly because an EDR is not a plug-and-play solution.

Aligning default EDR policies to organizational needs and building an adequate rule-base takes time. Defining the scope of telemetry, deciding what threats to detect first, identifying what assets to protect first are challenging. So talented, experienced staff is really needed and it is not easy to find and retain them. Moreover, frequent turnover appears to be another obstacle if we can find the talented staff, because they may quit for various reasons like pay rise offer from a rival company.The average duration of employment is predominantly less than five years according to a recent SANS report I have read. Talent pool is still not adequate and finding and also retaining skillful staff is a major problem.

Also if a talent is given inadequate salary, then he/she may quit and it can be difficult to find a replacement. Teams in SOC must regularly rank cybersecurity threats in terms of potential damage so they need to have the wide knowledge on various areas of cybersecurity. If they have the knowledge and the required experience, then they can prioritize the tasks in SOC. Moreover, only talented and experienced SOC teams can rapidly identify and remediate attacks to minimize the impact of cyber threats on the companies. If your response to a cyber attack is too slow, then, the impact of the cyber attack is more destructive and bad for your reputation as well.

Solutions:
SOCs rely heavily on the knowledge of individual cybersecurity team members. So talented cyber security experts should be found and also help to train new staff under experienced SOC analysts' supervision. Managers should provide ongoing training to stay on top of emerging threats, cybersecurity incident reports and vulnerabilities. SOC monitoring tools should be updated to reflect any changes by the talented/experienced staff. Lastly, management should create an environment where their staff is happy and willing to stay. Career mentorship, career opportunities can also help to encourage the staff. Happy staff can stay and train new comers and build a family-like working environment in a professional setting.

....................................................................

- "Problem: Alert Fatigue". Too many alerts are generated by our SIEM, EDR tools and also nearly half of them are false positives (according to the Ponemon Institute). So our SIEM users can't look into all of them and also the lack of correlation among alerts can cause tiredness among our SOC staff/users. We need to combat alert fatigue to accelerate threat detection and response capabilities of our Security Operations Center.

Moreover, we should reduce the burden on our staff caused by alert fatigue of SIEM tools.Their attention can be negatively affected by too many alerts when they do not provide real value and context. In short, we can validate the alert rules in our SIEM/EDR and identify detection gaps with the detection analytics feature of SIEMs. The Picus Security Control Validation Platform has these capabilities because after watching Purple Academy Training videos, I also used the 14 days trial and examined the capabilities and liked the contextual alert rules which can overcome the issue of the possible detection gaps. Furthermore, the video explained the need for a transaction form a reactive SOC to proactive SOC because proactive SOC provide contextual and necessary logs. So it mitigates the alert fatigue and this helps our SOC team and their performance.

If we can find a proper solution to alert fatigue and decrease the number of false or positive alarms, we can also decrease the process latency. Last but not the least, if we have many unrelated and minor logs, it can also cause other problems, not relevant to this question, tough. ( like logs in size of 10 Terra bytes can tire the computing power and cause extra expenses)

..............................................

 _(Since we are asked to write 5 at most, I will try to blend some related issues and do my best to integrate and show their connection as a whole. Otherwise, I needed to write/reply 6-7 issues:)   [Please write at most five prioritized issues]_
 
- "Problem: Technology" Technology also creates challenges for SOC teams. Lack of adequate tooling, lack of automation and integration, inadequate analytics and filtering, lack of enterprise-wide visibility and lack of proper log management in a contextual way".
This can also lead to serious problems which we obviously do not want. Lack of context can result in omitting some possible serious findings in our logs. Humans need a context to understand in a more efficient and meaningful way.

For possible solutions, automation and orchestration and tools' integration is needed. Too many tools that are not integrated is a problem and automation and orchestration can help to overcome this issue if we have skillful/trained staff. And these staff will need actionable alert rules and access the required log sources which will enable fast response to the detection gaps in user's environment. Technology is great when used properly but also without validations, needs analysis, they can be an obstacle as well. So we need metrics to test and validate our current tech usage.Testing and validating rules are also important to find whether the rule can detect the intended threat and whether it gives false positive or false negative results. That is how we can decrease our response time by the proper use of tech fine tuning.

In short, metrics are a critical component of the SOC’s interaction with the organization. Yet, most of the metrics used fail to effectively characterize the value the SOC provides to the business. Therefore, we need to increase the enterprise-wide visibility by proper metrics. We live in a data-driven world in a way and the future will be based on data science. So, we need to have the right metrics and validate these metrics as well. Our metrics can also give us the answers of these questions:"Is our technology working? What’s effective?, What is ineffective".

To remediate the drawbacks:
Firstly, we should identify the logs to have the required data visibility for threats. Then we can identify built-in but not activated rules by the vendor of the EDR.
We can develop our own rules if we have the required resources, or we can utilize from other libraries. In Picus Security Purple Academy videos, it is explained well how  Picus Mitigation Library can help for this purpose, so in order not to write a very long answer, I'll keep it short here by saying Picus provides a rich threat context for cyber defense teams by giving up-to-date Threat Intelligence ready to use.

By choosing right tools like Picus BAS, we can overcome the challenges technology also causes. As I said at he very beginning, technology also creates challenges for SOC teams and remediation to these challenges when used properly by talented/experienced staff.Breach and Attack Simulation(BAS) platforms like Picus can improve EDR Solutions and compensate some of the EDR drawbacks.

By using BAS platforms like Picus BAS, users can validate collected logs, identify logging gaps, and pinpoint required log sources. Users can also validate the alert rules of their detection systems, and identify detection gaps with the detection analytics feature of the Picus platform. So, using the platform, they can identify the gaps in their detection and also prevention. Measuring and minimizing the time gaps are critical especially in times of intense cyber attacks.

Lastly, prior to establishing a SOC, an organization must define its cybersecurity strategy to align with current business goals and problems and know what technology is needed beforehand. That is why we need enterprise wide visibility and validate our metrics, hence we can better evaluate ourselves by solid metrics to overcome these issues and mitigate the problems that SOC users face.

 
My answer to this question "What are the possible results and changes in the organization using the solution?" is:

By the help of the needed tools, proper metrics and validation of our metrics we can have a better assessment of the trends in cybersecurity, current cyber threats, provide better service to our users/customers and a have better share in the market. So we need to ask ourselves "Do we use the necessary tools properly?", "Are Trends in technology/cybersecurity going in the right direction?"

If we do not have proper tech stack to cope with logs, proper log management, proper threat intelligence and enterprise wide visibility, then we will end up in business blindness which will cause many issues for us. For example, if we blindly follow trends in cybersecurity and trust 100%, then we may tend to follow a possible wrong path. We need to access the effectiveness and success of various trends. We can define and track the critical metrics to our organization and thus we can ensure that our organization are going in the right direction.


...........................................

- "Problem: Lack of budgeting or Budgets spent ineffectively" A realistic model of required investment should be developed and necessary investment should be provided. Besides, management and SOC leads/managers ought to work together closely to decide how to allocate funds for cybersecurity. From the reports I have read, I can say that management tend to take recommendations from SOC leads/managers but frequently goes against SOC management’s recommendations. Thus this can be a issue because this can de-motivate the SOC team and users of SOC can be adversely affected as a result. After watching Picus Purple Academy Videos, I have seen how valuable and effective that Picus Breach Attack Simulation platform is. So if I were a SOC analyst, I would obviously utilize this software because it can simulate the cyber attacks in a risk free way, shows the gaps in log management systems and help the blue team a lot. However, I guess, the company management will tend to ignore SOC users' recommendations for financial reasons. Also many CEO, CTO will understand the importance of these after a breach, cyber attack, unfortunately. So, although, in the Purple Academy videos, lack of budgeting is not mentioned, I do believe it is an issue that SOC teams/users experience as a problem. SOC team and SIEM, EDR tools cannot collect and analyze all log sources because of costs and performance issues, so investing on a Breach Attack Simulation solution by a pioneer company like Picus can be a great solution. When ,for example, I try to explain this to a director in the company, I may hear "We do not have budget for it at this moment". So, if I were a user or a staff in SOC, I would see "Lack of Budgeting" as a problem

Solution:
We need to make sure our organizational management listens to SOC users' feedbacks, suggestions so the budget is not allocated on the wrong basis. We should focus on mitigating the threats with the greatest potential for damage so budget planning has to be flexible according to necessity. To effectively protect the enterprise, SOC teams need tools that enable them to maximize the effectiveness of their limited teams and resources. Hence, budget planning should take this into account Lastly, budgeting is important because there is a big competition among cybersecurity companies. If you do not spare enough financial resources or spend wrongly, then you will suffer from the rivalry and lose your market share and investors. In business life, the investors want to be given valid reasons for the expenses. We need to take into account that we live in a global world and the business has changed a lot. Our mistake can decrease the company value dramatically in a day in the stock market. So there is no need to say that budgeting is of vital importance not only in cyber security companies/start-ups but also in business in general.



NOTE to the exam evaluator: There are some other things to consider. However, since we were supposed to write 5 at most, I did not mention them and tried to order the 5 issues according to their importance or what I think about them after watching Picus Security Purple Academy videos. If we were supposed to write 6-7 issues, then I would also mention compliance maintenance since it is also important legally because companies must follow regulatory and organizational standards when carrying out business plans and SIEM operations. One operation can be permitted in the USA but not in Europe when GDPR is taken into account.




