# Maven-notes
Maven 3 notes with IntelliJ IDEA 14

# Contents
1. [What?](what)
  1. (Structure of Maven)[#structure-of-maven]
2. [How?](how)
  1. [Struct of each project](#structure-of-each-project)
3. [Opening Maven projects in IntelliJ IDEA](#opening-maven-projects-in-intellij-idea)
  1. [Traditional method](#traditional-method)
  2. [Using Maven's pom.xml](#using-mavens-pomxml)

## What?
An introduction to maven can be found on their website [here](http://maven.apache.org/what-is-maven.html).
### Structure of Maven
<pre>
project_folder
|
+-- src
|   |
|   +-- main
|   |   |
|   |   +-- java
|   |   `-- resources
|   `-- test
|       |
|       +-- java
|       `-- resources
+-- target
`-- pom.xml
</pre>

## How?
To create a maven project do the following

1. Click on `Create New Project`
2. On the left side of the `New Project` window click on `Maven`, then click `Next`.
3. This will take you to a new page enter your details. For example:
<pre>
GroupId: come.gollahalli.main
ArtifactId: project_folder
Version: 1.0-SNAPSHOT
</pre>
Then click on `Next`.
4. This will take you to a different page, enter your details. For example:
<pre>
Project name: project_folder
Project location: ~/some_location/project_folder
</pre>
click on `Finish`.

This will create the following structure

### Structure of each project
Every project created with Intellij 14 (using Maven) in this tutorial will have the following files and folder (any text below without extension is a folder).

<pre>
project_folder
|
+-- .idea
|   |
|   +-- copyright
|   |   |
|   |   `-- profiles_settings.xml
|   +-- .name
|   +-- compiler.xml
|   +-- misc.xml
|   +-- modules.xml
|   +-- vsc.xml
|   `--workspace.xml
+--src
|   |
|   +-- main
|   |   |
|   |   +-- java
|   |   `-- resources
|   `-- test
|       |
|       `-- java
+-- project_folder.iml
`-- pom.xml
</pre>

## Opening Maven projects in IntelliJ IDEA
There are two ways to open a project in IntelliJ (when using Maven).

### Traditional method
1. Launch IntelliJ IDEA 14 application and click on `Open`.
2. This will launch a file explorer, browse to the `project_folder` and click on `choose`.

> Note: This method will only open in IntelliJ IDEA environment.

### Using Maven's `pom.xml`
1. Launch IntelliJ IDEA 14 application and click on `Import Project`.
2. This will open an import file explorer, browse to `pom.xml` and click on 'OK'
3. This will import all the required dependancies and create all the folders required to run the project.
