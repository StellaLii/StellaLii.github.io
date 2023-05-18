---
layout:     post
title:      Working Sample
date:       2022-08-20
author:     Jianan
header-img: img/post-cars.jpeg
catalog: true
tags:
    - Python
    - Data Visualization
    - Machine Learning
---

# Working Sample

>Project Link: https://github.com/StellaLii/Simulation-Test-for-Planning-Module-Using-API, https://github.com/StellaLii/Auto-Report-for-Test-drive-Vehicle-Usage-and-New-Bug-Control

## Our Test Procedures
### 1 Unit Tests
Planning algorithm developers are responsible for this part. making sure individual components of the planning module are tested separately to ensure they are functioning as expected.

### 2 Integration Tests
Integration tests is to ensure that the different parts of the module interact correctly with each other. If there is crash happening, we need to consider the compatibility issues.

### 3 Simulation Testing
I am fully responsible for simulation testing. Simulation Testing includes three parts components. Simulation testing is using a simulated environment to test the planning module.

#### 3.1 Version Comparison
![UML](/picture/WorkingSample/VersionCompare.jpg)
This involves conducting a detailed comparison between the old and new versions of our algorithm. Different types of scenarios are invlved, including both common and edge cases, to evaluate the software's responses.
#### 3.2 New Implementation
When a bug fix is implemented, I use specific scenarios in the simulated environment to ensure that the previously identified issues have been rectified.  
For feature enhancements, I execute regression tests to determine whether the intended improvements are tangible in the new version.
![UML](/picture/WorkingSample/RetroTest.jpg)
We use grading system to test the performance.

#### 3.3 New Issues that caused by the new implementation
Sometimes, new implementation will cause some new issues. I need to take a look on that. 

### 4 HIL Testing
HIL Testing is tested in controlled real environment using actual hardware components by hardware team.

### 5 Real-world Testing
After the planning module passes the earlier testing phases, it is installed in an actual self-driving vehicle and tested in real-world driving conditions. The car's responses are monitored closely, and any inconsistencies or errors in the planning are noted for further improvement.  
All inconsistencies, unreasonable behavior, and drivers engagement cases will be recorded and sent to the database for furthur investigation. 
![UML](/picture/WorkingSample/NewIssues.jpg)

### 6 Grading for New Issues
For new issues, we need to use our grading system to add metrics to each scenarios based on their types. The metrics will help us automatically test the software's performance.         
**Nominal Evaluation**   
Stopping simulation    
SDC hard brake reaction point   
Cut-in Evaluation   
Tailgater reaction times   
VRU react to the SDC   
Exhibited reaction stopping simulations   
Swerving model   
Safety-related buffers   
