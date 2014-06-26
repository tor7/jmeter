comp412
=======================
*Week 3*:

Preliminary Draft
======================
Project name
-----------------
JMeter: User Interface (UI) enhancement(s)

>###Introduction
The Apache Software Foundation (ASF) manages more than 139 projects including Apache JMeter. "The Apache JMeter desktop application is open source software, a 100% pure Java application designed to load test functional behavior and measure performance." It can be utilized to test the different type of connections such as HTTP; LDAP; database connection using JDBC; TCP; and other connections. Plugins are the fundamental parts of the JMeter’s architecture. In other words, it can be extended by developing the customized plugins.

###Goals:
 - get familiar with JMeter
- improve user experience
- verify user’s test scenarios
- fix Bug #54784
- fix Bug#54525 –optional
- test the proposed bug-fix(s) on various browsers (e.g. Internet Explorer, Firefox, and Chrome)

###Scope
Implement solution to fix the Bug #54784, write detailed documentation, create a patch and try to submit it for approval.
If patch is accepted and we have enough time-we can try to take a look at [enhancement request #54525](https://issues.apache.org/bugzilla/show_bug.cgi?id=54525)
There are rules for patch creation, doc writing etc. It would be a fun time to get familiar with those requirements. The idea here is to get involved in a FOSS development process and to contribute.

###Bug description
There is a selection/add issue while using the “Enter” button to select/add the desired option from the right-click menu.

###Bug Background

*Bug #54784*:
The bug description and test scenario have been provided as stated below: “User cannot use the right-click menu fully with keyboard navigation.
    Launch JMeter
    Select a Thread Group
    Press Shift+F10
Result: Nothing happens
Expected: That the right-click menu is displayed, as in other Windows applications.
    Right-click on the Thread Group
    Navigate with keyboard arrow buttons to an element, e.g. Add, Sampler, HTTP Request
    Press Enter on keyboard
Result: Nothing happens.
Expected: That the selected element is inserted”
Benefits: better user’s experience

*Bug #54525*:
          Related issue(s): [Bug#22076](https://issues.apache.org/bugzilla/show_bug.cgi?id=22076)
User described this issue as stated below:
“The ability to search and replace when creating new variables would be very useful. 

It would be an even greater enhancement if there were a button available on the User Defined Variables form that would allow me to:

‘Find any occurrences of the [MYVALUE] string and replace with '${[MYVARNAME]}'".
Benefits: saving the time, risk and effort of having to go through the plan and complete this process manually’. “

###Hardware description
The preliminary bug verification will be performed on Windows 7 Home Premium (x64-bit, Intel Core i7), Windows 7 Professional (x64-bit, Intel Pentium).

###Priority
Bug #54525 - P2 enhancement
Bug #54784 - P3 enhancement

##Ruling
Follow the User’s Guide instructions to get familiar with the Apache JMeter.
Get familiar with the distributing testing, recording tests.
Review the JUnit Sampler and Access Log Sampler sections
Follow the steps (if applicable) described in The Contributors Tech Guide (e.g. Sending in Patches) https://www.apache.org/dev/contributors 
The enhancement implementation process is guided by Contributors Tech Guide 

###Authorized persons
Tianlin Cai
Viktor P Titenko

###Duties
>***Viktor P. Titenko***:
-	Create a trello board for collaboration
-	Come up with idea for FOSS project
-	Create a draft for project proposal 
-	Create a GitHub repository for FOSS team project
-	Clone/fork the Apache JMeter into GitHub account
-	Perform the code review
-	Install JMeter on the local machine
-	Start JMeter
-	Visually check/confirm the reported defect (enhancement request)
-	Run one or two tests to make sure that the JMeter is working
-	Identify/locate the project package(s) to start work on
-	Create a step-by-step plan to fix Bug #54784 
-	Create the Test Plan to test modified package(s)
-	Create the Test Strategy (e.g. types of tests to perform – functional, non-functional tests, etc)
-	Create a Test Case(s)
-	Run Test Case(s)
-	Create a screencast
-	Add additional duties if needed
-	Write Documentation page(s) as needed

>***Tianlin Cai***:
-	Post the project idea on the facebook page
-	Create a new Card for project proposal
-       Add Markdown syntax to project proposal
-	Join the Apache JMeter Mailing List if needed
-	Try to communicate to the project community when initial goal has been reached (.e.g. get familiar with the JMeter) – Feel free to modify/delete this statement 
-	Add more duties to this paragraph
-       Clone/fork the Apache JMeter into GitHub account
-	Perform the code review
-	Install JMeter on the local machine
-	Start JMeter
-	Visually check/confirm the reported defect (enhancement request)
-	Run one or two tests to make sure that the JMeter is working
-	Identify/locate the project package(s) to start work on
-	Create a step-by-step plan to fix Bug #54784 
-	Create the Test Plan to test modified package(s)
-	Create the Test Strategy (e.g. types of tests to perform – functional, non-functional tests, etc)
-	Create a Test Case(s)
-	Run Test Case(s)
-	Create a screencast
-	Add additional duties if needed
-	Write Documentation page(s) as needed

**Test Results Analysis**
Confirm that the issue has been fixed
Create a screenshot

**Risks and Mitigation**
Provide additional information about the cross-browser issues (if any) for further references

**Project Milestones**
Configure JMeter to run locally
Discover the way(s) to fix the issue(s)

**References**
[User Manual](https://jmeter.apache.org/usermanual/)
[Contributors Tech Guide](https://www.apache.org/dev/contributors)
[Get Involved](https://www.apache.org/foundation/getinvolved.html)

