# threatmodeling-resources
## Introduction
Threat Modeling is often considered a key activity in the SDL (Secure Development Lifecycle). 
Threat modeling is a family of activities for improving security by identifying objectives and vulnerabilities, and then defining countermeasures to prevent, or mitigate the effects of, threats to the system. A threat is a potential or actual undesirable event that may be malicious (such as DoS attack) or incidental (failure of a Storage Device). Threat modeling is a planned activity for identifying and assessing application threats and vulnerabilities.


Feel free to use the following poster in your threat modeling sessions. 
![Threat Modeling Steps](/images/threat_modeling_steps.jpg)
(c) Marlene Herr

## Steps
A more detailed step-by-step guide is soon to come. 
### Big Picture
Visualize the system architecture together with the team. You can prepare the big picture beforehand but we've experienced that you should always talk about it together with the team to make sure no connections to sorrounding systems are missed.
### Assets and actors
Specify the assets that the system posesses and the actors who use the system.
### Trust boundaries
In this step you should clarify whether the connection is trusted (green) or not trusted (red). See the illustration at step 1 and 3. 
### Identify threats
Identify threats based on the steps before. Specify them as a evil user story: 

> As _actor_ i am doing _attack_ to damage _asset_

Try to be as specific as possible. Only then you can prioritize and mitigate the threat. A user story like 
> As an attacker i ddos the service

Is to broad and very hard to find a specific countermeasure for. 
### Prioritize threats
Priorization is an important step to make sure you only spend time on discussing the most relevant threats. The prioritization criteria will be added and explained soon. 
### Mitigate threats
Based on the most critical criteria you should find a mitigation to lower the risk. For example, if the most critical behaviour is the discover & response criteria, your main goal should be to get better in discovery/monitoring and responding to that threat.
### Next steps
The biggest part of next steps is the documentation and also implementation of your countermeasures. 

## References
- https://www.owasp.org/index.php/Category:Threat_Modeling
- https://www.microsoft.com/en-us/securityengineering/sdl/threatmodeling