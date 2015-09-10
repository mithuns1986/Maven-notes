# Contents

<pre>
1_HelloWorld
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
|   |   |   ` Main.java
|   |   `-- resources
|   `-- test
|       |
|       `-- java
+-- 1_HelloWorld.iml
`-- pom.xml
</pre>

## Dependencies

To add external libraries (dependencies) you would have to search them in maven repositories, best place to search dependencies can be found [here](http://mvnrepository.com/) and [here](http://search.maven.org/).

1. Search for the required dependency.
2. The copy the dependency xml code. For example
<pre>
<dependency>
    <groupId>joda-time</groupId>
    <artifactId>joda-time</artifactId>
    <version>2.2</version>
</dependency>
</pre>
3. Next open `pom.xml` file from the project and type the following xml code
<pre>
<dependencies>

</dependencies>
</pre>
inside `<project>...</project>`
3. Then paste the copied xml code inside `<dependencies>` tag. For example
<pre>
<dependencies>
    <dependency>
        <groupId>joda-time</groupId>
        <artifactId>joda-time</artifactId>
        <version>2.2</version>
    </dependency>
</dependencies>
</pre>