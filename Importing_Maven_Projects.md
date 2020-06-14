# Importing Existing maven projects in various IDEs

## Netbeans (8.2)
To open a maven project in netbeans you can either open your project folder (the one containing the POM.xml) directly as a project with the `File > Open Project ...` menu

or

you can create a new project, select the Maven category, and choose "Project with Existing POM" - which then prompts you to select the project folder like before.

## Eclipse 
* Open eclipse
* Ensure you have the Maven Support Plugin
  * Click Help > Install new software
  * Enter https://download.eclipse.org/technology/m2e/milestones/1.15/
  * Select "Maven Integration for Eclipse"
  * Click Next as many times as required.
* Click File > Import
* Type Maven in the search box under Select an import source:
* Select Existing Maven Projects
* Click Next
* Click Browse and select the folder that is the root of the Maven project (probably contains the pom.xml file)
* Click Next
* Click Finish
* Run the project for the first time and enter the goal `clean install` or `clean compile` as you prefer for the default goal. (install will add the project to your local maven repo to allow use as a dependency - as well as all intermediate goals)


## IntelliJ 
To open the Maven project, just go to `File > Open Project` (Alt + F + O) and specify the path to pom.xml (the Maven project descriptor file).

When done, all maven goals can be found in the Maven Projects tool window. You can run/debug arbitrary Maven goals; execute them before/after make or run/debug.

## VS Code
Why you've chosen this IDE for this task is beyond me, but here's a [post describing how set up VSCode to accept maven projects.](https://stackoverflow.com/questions/46671308/how-to-create-a-java-maven-project-that-works-in-visual-studio-code).

Alternatively, there is an Extension that claims to do this for you [here](https://marketplace.visualstudio.com/items?itemName=vscjava.vscode-maven).

I cannot attest to the function or usefulness of either approach.
