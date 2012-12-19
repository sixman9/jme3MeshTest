# jme3MeshTest

This project serves as a proof of concept of the retrieval and integration of Maven-repository-distributed [jMonkeyEngine 3][3] (jme3) Java libraries into a [Gradle][1] managed [Groovy][2]-based build script. This jme3 and [Gradle][1] test project uses the **[jme3test.model.shape.TestCustomMesh][4]** test class, just type **'gradlew'** to run it.

Running **'gradlew'** or **'gradle'** [if installed] is enough to execute the default tasks (build, runJar).  
  
For IDE project setup, run **'gradle[w] eclipse'** OR **'gradle[w] idea'**, e.g. **gradlew idea**. After, import the new project into your IDE (all libraries, source and classpaths will be resolved).  

# About Gradle

[Gradle][2] takes advantage of a fully-fleged Java-compatible programming language, [Groovy][2], while extending Ant-sourced project build techniques and Maven-like distributed code repository library management. Basically it's like Ant and Maven rolled into one while letting you write 'FOR' loops and 'CASE' statements or programatically scraping a webpage or writing a file in the middle of a build!

Although [Gradle][1] is [Groovy][2] based, [Gradle][1] can be self-distributing via its 'wrapper' task. This means that a Gradle-built project, such as this one, can be built straight after checkout, as long as a JVM is present (i.e. no Gradle install required!).

**output from 'gradle tasks':**

Application tasks
-----------------
**distZip** - Bundles the project as a JVM application with libs and OS specific scripts.  
**installApp** - Installs the project as a JVM application along with libs and OS specific scripts.  
**run** - Runs this project as a JVM application

Build tasks
-----------
**assemble** - Assembles the outputs of this project.  
**build** - Assembles and tests this project.  
**buildDependents** - Assembles and tests this project and all projects that depend on it.  
**buildNeeded** - Assembles and tests this project and all projects it depends on.  
**classes** - Assembles the main classes.  
**clean** - Deletes the build directory.  
**jar** - Assembles a jar archive containing the main classes.  
**testClasses** - Assembles the test classes.  

Documentation tasks
-------------------
**javadoc** - Generates Javadoc API documentation for the main source code.  

Help tasks
----------
**dependencies** - Displays all dependencies declared in root project 'jme3MeshTest'.  
**dependencyInsight** - Displays the insight into a specific dependency in root project 'jme3MeshTest'.  
**help** - Displays a help message.  
**projects** - Displays the sub-projects of root project 'jme3MeshTest'.  
**properties** - Displays the properties of root project 'jme3MeshTest'.  
**tasks** - Displays the tasks runnable from root project 'jme3MeshTest' (some of the displayed tasks may belong to subprojects).  

IDE tasks
---------
**cleanEclipse** - Cleans all Eclipse files.  
**cleanIdea** - Cleans IDEA project files (IML, IPR)  
**eclipse** - Generates all Eclipse files.  
**idea** - Generates IDEA project files (IML, IPR, IWS)

Verification tasks
------------------
**check** - Runs all checks.  
**test** - Runs the unit tests.  

Other tasks
-----------
**cleanIdeaWorkspace**  
**runJar** - Executes the bundled Jar artifact, equivalent to 'java -jar <executable>.jar'.  
**wrapper** - Creates a project-installed distribution of the specified Gradle runtime version (gradlew).  

[1]: http://www.gradle.org
[2]: http://groovy.codehaus.org
[3]: http://www.jmonkeyengine.org
[4]: https://code.google.com/p/jmonkeyengine/source/browse/trunk/engine/src/test/jme3test/model/shape/TestCustomMesh.java
