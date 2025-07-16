# Maven-notes
Maven 3 notes using IntelliJ IDEA 14

**License**

The code is provided under [MIT License](https://github.com/akshaybabloo/JavaScript-Tutorial/blob/master/LICENSE) and the tutorial is provided under [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License](http://creativecommons.org/licenses/by-nc-sa/4.0/)

![CC](https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png)

# Contents
1. [What?](#what)
  1. [Structure of Maven](#structure-of-maven)
2. [How?](#how)
  1. [Structure of each project](#structure-of-each-project)
3. [Opening Maven projects in IntelliJ IDEA](#opening-maven-projects-in-intellij-idea)
  1. [Traditional method](#traditional-method)
  2. [Using Maven's pom.xml](#using-mavens-pomxml)
4. [Structure of this tutorial](#structure-of-this-tutorial)

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

mkdir maven-demo

cd maven-demo/

mvn archetype:generate -DgroupId=com.mycompany.app -DartifactId=my-app -DarchetypeArtifactId=maven-archetype-quickstart -DarchetypeVersion=1.5 -DinteractiveMode=false

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

## Running Maven projects 
mvn package

cd target/my-app-1.0-SNAPSHOT.jar

ls -l  target/my-app-1.0-SNAPSHOT.jar

java -cp target/my-app-1.0-SNAPSHOT.jar com.mycompany.app.App

vim src/main/java/com/mycompany/app/App.java

java -cp target/my-app-1.0-SNAPSHOT.jar com.mycompany.app.App

mvn package

java -cp target/my-app-1.0-SNAPSHOT.jar com.mycompany.app.App

## Opening Maven projects in IntelliJ IDEA
There are two ways to open a project in IntelliJ (when using Maven).

### Traditional method
1. Launch IntelliJ IDEA 14 application and click on `Open`.
2. This will launch a file explorer, browse to the `project_folder` and click on `choose`.

> Note: This method will only open in IntelliJ IDEA environment.

### Using Maven's `pom.xml`
1. Launch IntelliJ IDEA 14 application and click on `Import Project`.
2. This will open an import file explorer, browse to `pom.xml` and click on 'OK'
3. This will import all the required dependencies and create all the folders required to run the project.

## Structure of this tutorial

1. [1_HelloWorld](https://github.com/akshaybabloo/Maven-notes/tree/master/1_HelloWorld) - is a basic java application using Maven.
