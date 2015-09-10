# Maven-notes
Maven 3 notes with Intellij 14

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

## Structure
Every project created with Intellij 14 (using Maven) in this tutorial will have the following files and folder.

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
|   |   |   |
|   |   |   `Main.java
|   |   `-- resources
|   `-- test
|       |
|       `-- java
+-- project_folder.iml
`-- pom.xml
</pre>
