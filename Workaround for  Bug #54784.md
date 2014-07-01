Project name
=======================
JMeter: User Interface (UI) enhancement(s)

----------------
*Week 3*:  Progress


>###Feature request validation [Bug #54784](https://issues.apache.org/bugzilla/show_bug.cgi?id=54784). 

The reported behaver of the right-click menu has been confirmed.
The "Enter" keyboard shortcut is not activated while the navigation arrow buttons are working fine.

>###JMeter Wiki info.
The requested feature (such as "Shift+F10") is not listed under the current JMeter KeyBoard Shortcuts' page.
However, the "F10" keyboard button invokes the "File" drop-down menu  which allows the further navigation by utilizing the keyboard arrows buttons

### *There is a workaround to achieve the requested functionality by utilizing the specific order of the current keyboard shortcuts.
It includes three basic steps.
First of all, user should select the desired element under Test Plan tree.
The second step is to press the "F10" button to invoke the pop-up of the File menu.
Third step is to pres the "right" keyboard arrow to navigate to the Edit Menu.
Finally, user can traverse/add all available options under Edit menu by utilizing the known keyboards shortcuts.

###Bug description
There is a selection/add issue while using the "Enter" button to select/add the desired option from the right-click menu.

###Bug Background
*Bug #54784*:
The bug description and test scenario have been provided as stated below: User cannot use the right-click menu fully with keyboard navigation.
    Launch JMeter
    Select a Thread Group
    Press Shift+F10
Result: Nothing happens
Expected: That the right-click menu is displayed, as in other Windows applications.
    Right-click on the Thread Group
    Navigate with keyboard arrow buttons to an element, e.g. Add, Sampler, HTTP Request
    Press Enter on keyboard
Result: Nothing happens.
Expected: That the selected element is inserted
Benefits: better user's experience

**Test Results Analysis**
The proposed workaround provides similar functionality

>**Additioanl information
Edit Menu implementation: *jmeter-->core-->org.apache.jmeter-->gui-->actions-->EditCommand.java*
**TODO**
Implement the requested feature
  "Shift + F10" to invoke the "Edit" menu while the "Thread Group" element is highlighted.

**Project Milestones**
Discover the package (and java classe(s)) that invoke/implement the right-click menu

**Reference(s)**
[JMeter Keyboard Shortcuts](https://wiki.apache.org/jmeter/JMeterShortcuts)




