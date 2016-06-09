Showcase - Faster and more efficient processes by combining BPM and Mobile
======================================================================

A. Synopsis
===========

What this is about
------------------
A lot has happened in the area of mobile since Apple kicked off the revolution by announcing the first iPhone. However, the overall mobile market still has to be considered as young and especially unstandardized. This really puts a lot of organizations in front of huge challenges concerning the efficient development of mobile applications and the secure integration into backend IT systems.

But there is no way around mobile in the next years! The smart combination of mobile techniques (mBaaS, micro services, etc.) and business process management approaches will definitely drive process efficiency and speed to a whole new level.

#### The use case or "What if the process was at the fingertips of your customer?"
This showcase addresses a scenario that almost all enterprises in the insurance industry are facing: Nowadays users expect to be able to contact their insurance 24/7 on an ad-hoc basis (e.g. for opening a claim or just for asking a question concerning their policy). Additionally they want to see on demand what the status on a certain request is. From an enterprise point of view insurances are looking at new ways on reacting to this new speed of communication and transparency. They're also thinking of new concepts to efficiently integrate agencies and remote workers in their existing processes. - They key answer to these requirements is to enhance existing input & output management infrastructure by a new mobile channel.

In this showcase we used Red Hat Mobile Application Platform ([https://www.redhat.com/en/technologies/mobile/application-platform](https://www.redhat.com/en/technologies/mobile/application-platform)) to efficiently and securely connect the outside world with existing enterprise systems.

![ARC_OVERVIEW - Use case](./doc/01_arc_overview_use_case.png)

Through the platform approach we do not need to reinvent the wheel for each mobile app on the horizon. Instead we established a centralized platform for developing and running mobile application in a standardized manner.

The use of Red Hat Mobile Application Platform (RHMAP) comes with the following benefits:
* Agile approach to developing, integrating, and deploying enterprise mobile applications—whether native, hybrid, or on the web
* Out-of-the-box automated build processes
* A service catalog for reusable connectors to backend
* Easy scale-out through cloud native architecture
* Collaborative development across multiple teams and projects with a wide variety of leading tool kits and frameworks

Architectural overview
----------------------
From a technical point of view the showcase is comprised of three main building blocks
1. CLIENT LAYER: Hybrid mobile applications running on the end user devices
2. CLOUD LAYER: Node.js based backend running in the cloud on RHMAP
3. BACKEND LAYER: Set of business process applications running on [JBoss BPM Suite](https://www.redhat.com/en/technologies/jboss-middleware/bpm) as the underlying BPM engine

![ARC_OVERVIEW - Component model](./doc/02_arc_overview_component_model.png)

#### Client layer
tbd

#### Cloud layer

##### Mobile backend as a service (MBaaS)
An MBaaS (Mobile Backend-as-a-Service) is the primary point of contact for end user applications - both mobile and web. The MBaaS hosts Node.js applications - as REST API servers and/or Express.js based web apps. The primary purpose of the MBaaS is to allow users (developers) of RHMAP to deploy Node.js server-side for their mobile apps. The MBaaS also provides functionality such as caching, persistence, data synchronization and a range of other mobile-centric functionality. Multiple MBaaS may be utilized for customer segregation and/or lifecycle management (environments).

Describe components...


##### Push network
More information on the push API can be found here [http://docs.feedhenry.com/v3/product_features/push_notifications.html](http://docs.feedhenry.com/v3/product_features/push_notifications.html)

Screenshots
------------------
tbd


Source code
-----------
The source code can be found here:
#### Client layer
* [Hybrid Customer App](https://github.com/Sifa91/fh-mobile-bpm-client-customer)
* [Hybrid Client App](https://github.com/Sifa91/fh-mobile-bpm-client-employee)

#### Cloud layer
* [RHMAP Cloud Application](https://github.com/sebastianfaulhaber/fh-mobile-bpm-cloudapp)
* [RHMAP MBaas BPM Connector](https://github.com/sebastianfaulhaber/fh-connector-bpm)

#### Backend layer
* [JBoss BPM Suite Request Processing Application](https://github.com/sebastianfaulhaber/fh-mobile-bpm-processapp)

B. Installation
===============

1. Red Hat Mobile Application Platform
--------------------------------------
There are multiple ways to s

2. JBoss BPM Suite
------------------

3. Configure push notifications
----------------------------

4. Setup local development environment
--------------------------------------


C. User guide
========================

1. How can I xyz?
--------------------------------------------------
tbd

D. Reference Information
========================

E. Credits
==========
Sebastian Dehn @Sifa91
