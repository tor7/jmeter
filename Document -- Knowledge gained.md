*Document -- Knowledge gained*
=======================
**JMeter: Knowledge gained when doing User Interface (UI) enhancement(s)**

----------------
*Targeted Enhancement*


>###Feature request validation Bug #54784 (https://issues.apache.org/bugzilla/show_bug.cgi?id=54784). 

The reported behaver of the right-click menu has been confirmed.
The "Enter" keyboard shortcut is not activated while the navigation arrow buttons are working fine.

>###JMeter Wiki info.
The requested feature (such as "Shift+F10") is not listed under the current JMeter KeyBoard Shortcuts' page.
However, the "F10" keyboard button invokes the "File" drop-down menu  which allows the further navigation by utilizing the keyboard arrows buttons

### *Despite Viktor and I didnt achieve the target to fix this bug, I learned something I felt useful when I was approaching the target*.
It includes the points below:

1. TestPlan and WorkBench GUI classes are loaded directly, so the display on the left tree menu of Jmeter also started both. It is default but you can edit the menu by changing the source code in MenuFactory.

2. Each Config Element, as long as the expansion from ConfigTestElement, its properties using the tool corresponding attribute BeanInfo class to be set; After attribute attributes, such as the default value of the property, whether to allow it is blank, You can use this property in the future, to obtain the corresponding constraint value, and its convenient for programming.

3. AbstractSampler class is really working, but it is not a visible device on the screen, which is correspond with Sampler Config Element and Sampler Default Config Element, it will perform sample method each time thread iteration. Return result SampleResult can call display for other components.

4. I use jmeter to record 127.0.01, recording unsuccessful, but the recording of Google and other sites are successful.
>###Cause
When I visit the local tomcat, the browser automatically skips the local proxy server, so the local script recording unsuccessful.
>###Solution
Record  scripts with badboy, verify the correctness of the script, and then export to jmeter test plan. 
Enable another server, enter the server IP and port number, visit its website.

5. Compare badboy script recording with Jmeter proxy sever script recording.
>###Advantage: 
Badboy can record the contents of the local server, and jmeter proxy server can not do that. 
Badboy script recording, simple, distinct, clear, able to play back the script, find an error from the script of the play. 
There are many errors for jmeter proxy server to record the script itself, and difficult to find, but badboy records content in the form of page, then more advantages on the error found . 
>###Disadvantages: 
Can not be parameterized and associated, these can only be achieved in the jmeter. 
Recorded script requires import and export, in the process, people do not know whether the contents of the script changed or errors occured, thus it is difficult to accurately locate errors in the test run.

6. Jmeter can store Cookie information corresponding to threads and apply that information in the script, there are no cookie situation and cookie situation. The role of the HTTP cookie manager is, for example, Sina Weibo user name and password are stored in the form of cookie, you must add these cookie, then you can log in Sina Weibo successfully.

