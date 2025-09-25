what it is? why we use it? how to implement

1.client/end user  2.server 3.API 4. Database
server is then divied into two psudo parts known as ends.
A. (i) base url (google.com) (ii) end-point
B. backend and database are connected via Driver, for mern it is mongoose(mongodb)

HOW? ->
Client -> ISP -> Server . this request has a protocol

**TCP/UDP** 
TCP -> end-to-end secure (whatsapp chat)
UDP -> no security

OG NAME OF JS - mocha
JS is not parsed
Tree shaking/dead code alogs
Deployment/hosting: 
React made public in 17


**VCS & CI/CD:**
SST(Single Source of Truth)
LVCS - Local Version Controlling System 
CVCS - Centerliazed Version Controlling System 
DVCS -  Distributed Version Controlling System (modern - allows accessing and uploading) - Git

Main code -> Branch -> Pull Raise (PR) -> Testing-> Merging
NOTE: the code that is uploaded second, can raise a Merge Conflict

It can be done by GIT



CI( continuous Integration) : Build and test code code whenever changes are added, helps find and fix problem

CD( Continuous Delivery) : prepares and releases the tested code to different environments, like testing or live system.

USES **Spiral Waterfall Model** 


process:
1. requirement gathering
2. continuous integration
3. continuous delivery


Chapter:6
Developer's Daily workflow:
4. Pull latest code
5. write and commit
6. Trigger pipeline
7. Deploy

**TO DELPOY USE: VERSEL**

chapter:7
Building a Typical CI/CD pipeline:
1. build stage
2. test stage (consistent result, after achieving 100% accuracy, move to step 3)
3. deploy stage

Pipeline - main file is treated at as a path. avoids maintenance -> minimal downtime 

Chapter:8
Real world impact: faster, safer web development
87% - Improved quality
90% early bug detection
50% reduced downtime
Daily frequent Deployments

QUES. WHAT IS CI/CD PIPELINE?
	Throttling and debouncing