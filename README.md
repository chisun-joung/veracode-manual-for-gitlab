# Veracode-manual-for-GitLab



## Introduction  
This documentation should help Veracode customers to understand how they ca integrate Veracode scanning technologies into GitLab. It is almost universal to many other CI/CD tools, but this documentation is mainly focused on GitLab and it's specifics.  
Using this documentation you will be able to automte static, SCA and dynamic scanning from within your GitLab pipeline. As well you will learn how to scale application security testing in a larger organization with a lot of repositories. 


## Veracode Scanning Techologies
**Static Analysis**  
### Static analysis - SAST  
Veracode offers 3 types of static analysis  
1. Pipeline Scan 
2. Sandbox Scan  
3. Policy Scan  
  
All 3 are run on different needs and have different purposes, all are based on the same engine in the background and all 3 should find the exact same results if the same binary is uploaded.  

1. Pipeline Scan  
The Veracode Pipeline Scan was desgined as a fast feedabck tool for developers and may runs with every single commit. It can rate in very early stages what are the policy relevant findings a developer need to fix in order to achieve policy compliance later on. As well it gives you the possibility to see net-new findings of a single commit.  
It can scan the full application or smaller parts that have canged.  
  
2. Sadbox Scan  
Similar to the Pipeline Scan, the Sdandbox scan runs in early stages of your code. It's puprose is to scan the full application and rate the findings according to the profile's policy. This will allow you to see findings that need to be fixed in order to achieve policy compliance later one.  
  
3. Policy Scan  
The Policy Scan is the last gate to production. It should scan the full application and according to the policy compliance you can decide wether the application is allowed to be deployed or not.  

**Software Composition Analysis**  
Software Composition Analysis at Veracode can be done in 2 different ways.  
  
1. With static analysis (Upload and Scan)  
2. Individual SCA scan of the application and docker containers (Agent Based Scan)  
  
On this documentation we will mainly talk about the Agent Based Scan, that could run on every stage of your code.  

**Dynamic Analysis**  
Veracode#s Dynamic Analyssis gives you the possibility to scan standard or single page web applications and as well API's while they are running either at a stageing environment or at production.  
Both types of scan will be run and configured the exact same way.  
  
## Automation Process  
The picture below should highlight in a visual way whcih scan type runs at which stage of your code. It also is "only" Veracode's idea how it makes sense to impletment a good process to application security testing.  
Every organization is doing this a bit differently, depending on how their processes are set up. Veracode gives you the felxibilitxy to choose which scan type should run where on your different stages of your pipeline and your code.  
  
PICTURE PROCESS


## Pre-built docker images


## Integratiing into GitLab

### Scanning  
**Static Analysis**

**Software Composition Analysis**

**Dynamic Scanning**

### Reporting
**Static Scan Reporting**

**Software Composition Analysis Reporting**


## Scaling in an organization

### Templating



