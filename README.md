Minimal child pom:

```
#!xml

<?xml version="1.0" encoding="UTF-8"?>
<project xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns="http://maven.apache.org/POM/4.0.0"
         xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
    <modelVersion>4.0.0</modelVersion>

    <parent>
        <groupId>hzg.wpn.tango</groupId>
        <artifactId>server-parent</artifactId>
        <version>1.6</version>
    </parent>

    <artifactId>TestServer</artifactId>
    <version>1.1-SNAPSHOT</version>


    <properties>
        <scm.developerConnection>${scm.developerConnection.prefix}${scm.project.name}</scm.developerConnection>
    </properties>

    <scm>
        <developerConnection>${scm.developerConnection.prefix}${scm.project.name}</developerConnection>
    </scm>

    <build>
        <plugins>
            <plugin>
                <artifactId>maven-assembly-plugin</artifactId>
                <configuration>
                    <skipAssembly>false</skipAssembly>
                </configuration>
            </plugin>
        </plugins>
    </build>

</project>
```