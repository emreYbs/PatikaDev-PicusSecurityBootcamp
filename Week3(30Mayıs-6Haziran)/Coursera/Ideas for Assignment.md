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

