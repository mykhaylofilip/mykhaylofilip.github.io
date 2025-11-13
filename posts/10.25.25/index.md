<link rel="stylesheet" href="/assets/css/custom.css">

# Major AWS Outage – October 2025  
I would first of all like to mention this will be my first current event post on my website. I hope anyone who reads it finds it interesting. :D

On October 20, 2025, Amazon Web Services (AWS) suffered a massive outage in its US‑EAST‑1 region that disrupted hundreds (if not thousands) of websites and services worldwide.

The root cause? A DNS resolution failure in AWS’s DynamoDB service and a cascading chain of dependencies that broke down load‑balancing and compute capacity.

### What happened  
- The issues began around the early hours (US time) with failures in DynamoDB’s DNS system. 
- Because many other AWS services route through that region and rely on those databases, a domino effect occurred: EC2 instances couldn’t be launched, network load balancers failed, and many client services went offline.  
- The disruption lasted over 15 hours for full recovery in many areas — a reminder that even large cloud providers are vulnerable. 

### Why it matters  
For someone working in cybersecurity or system administration (like me), the outage illustrates:  
- The risk of **single‑region dependence**: even if your system is in another region, if your control plane depends on US‑EAST‑1 you may still be affected.  
- The importance of **multi‑region or multi‑cloud architectures**, especially for critical services or infrastructure.  
- That failures don’t always come from “attackers” — sometimes infrastructure errors cause major damage just as easily.
- I was actually doing the New Jersey Space Grand Challange, and some of the rooms/challange wouldnt work during this outage.   

### My takeaway  
This event pushed me to revisit how I deploy lab systems and prepare backups. Things I’m doing:  
- Checking where my control services run (region, provider).  
- Ensuring snapshots or backups of critical lab VMs are usable if one region is disrupted.  
- Practicing resiliency and restoration work so I’m prepared when something fails, not just assuming “it will never happen.”  

[Read more](https://www.wired.com/story/amazon-explains-how-its-aws-outage-took-down-the-web)  
