# Bildschirmarbeiter Checkstyle

Checkstyle checks for Bildschirmarbeiter projects

* [Checkstyle](https://checkstyle.org)
* [Apache Maven Checkstyle Plugin](https://maven.apache.org/plugins/maven-checkstyle-plugin/)


## Usage

```
  <build>
    <plugins>
      <plugin>
        <groupId>org.apache.maven.plugins</groupId>
        <artifactId>maven-checkstyle-plugin</artifactId>
        <version>3.1.2</version>
        <dependencies>
          <dependency>
            <groupId>com.puppycrawl.tools</groupId>
            <artifactId>checkstyle</artifactId>
            <version>9.0</version>
          </dependency>
          <dependency>
            <groupId>de.bildschirmarbeiter</groupId>
            <artifactId>checkstyle</artifactId>
            <version>3</version>
          </dependency>
        </dependencies>
        <configuration>
          <configLocation>checks.xml</configLocation>
        </configuration>
        <executions>
          <execution>
            <phase>validate</phase>
            <goals>
              <goal>check</goal>
            </goals>
          </execution>
        </executions>
      </plugin>
    </plugins>
  </build>
```
