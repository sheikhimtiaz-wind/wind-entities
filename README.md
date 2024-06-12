# Wind Entities

== Installation

To use WindEntities in your project, you can add it as a Maven dependency.

[source,xml]
----
<dependency>
  <groupId>com.sheikhimtiaz</groupId>
  <artifactId>wind-entities</artifactId>
  <version>1.0.0</version>
</dependency>
----

For secure packages, here is the config

.m2/settings.xml -> 

<settings xmlns="http://maven.apache.org/SETTINGS/1.1.0"
xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
xsi:schemaLocation="http://maven.apache.org/SETTINGS/1.1.0 https://maven.apache.org/xsd/settings-1.1.0.xsd">
<servers>
<server>
<id>wind-artifactory</id>
<username>${env.MAVEN_USERNAME}</username>
<password>${env.MAVEN_PASSWORD}</password>
</server>
</servers>
</settings>


In the pom.xml file ->

    <repositories>
        <repository>
            <id>hilti-artifactory</id>
            <url>https://hilti.jfrog.io/artifactory/git-maven-virtual/</url>
        </repository>
        <repository>
            <id>central</id>
            <url>https://repo.maven.apache.org/maven2</url>
        </repository>
    </repositories>

    <dependencies>
        <!-- Your dependencies here -->
    </dependencies>


Set the credentials -> 

export MAVEN_USERNAME=yourUsername
export MAVEN_PASSWORD=yourPassword

