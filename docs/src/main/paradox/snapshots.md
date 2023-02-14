---
project.description: Snapshot builds of Apache Pekko Persistence JDBC are provided via the Apache snapshot repository.
---
# Snapshots

[snapshots]:        https://https://repository.apache.org/content/groups/snapshots/org/apache/pekko/pekko-persistence-jdbc_2.13/

Snapshots are published to the Apache Snapshot repository every night.

@@@ warning

The use of Pekko SNAPSHOTs, nightlies and milestone releases is discouraged unless you know what you are doing.

@@@

Add the following to your project build definition to resolve Apache Pekko Persistence JDBC's snapshots:

## Configure repository

Maven
:   ```xml
    <project>
    ...
      <repositories>
        <repository>
            <id>snapshots-repo</id>
            <name>Apache snapshots</name>
            <url>https://repository.apache.org/content/groups/snapshots</url>
        </repository>
      </repositories>
    ...
    </project>
    ```

sbt
:   ```scala
    resolvers += "Apache Nexus Snapshots".at("https://repository.apache.org/content/repositories/snapshots/")
    ```

Gradle
:   ```gradle
    repositories {
      maven {
        url  "https://repository.apache.org/content/groups/snapshots"
      }
    }
    ```

## Documentation

The [snapshot documentation](https://pekko.apache.org/docs/pekko-persistence-jdbc/snapshot) is updated with every snapshot build.

## Versions

Latest published snapshot version is [snapshots]

The snapshot repository is cleaned from time to time with no further notice. Check [Sonatype snapshots](https://repository.apache.org/content/groups/snapshots/org/apache/pekko/pekko-persistence-jdbc_2.13/) to see what versions are currently available.
