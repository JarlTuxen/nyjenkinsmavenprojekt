# nyjenkinsmavenprojekt

Dependencies for JUnit5 kan ses i pom.xml

De vigtige for JUnit5 er
* junit-jupiter-api som gør det muligt at skrive tests
* junit-jupiter-engine som kører unit tests
* maven-surefire-plugin som gør det muligt for Maven at finde og køre unit tests

```
<dependencies>
    <dependency>
        <groupId>org.junit.jupiter</groupId>
        <artifactId>junit-jupiter-api</artifactId>
        <version>5.4.2</version>
        <scope>test</scope>
    </dependency>
    <dependency>
        <groupId>org.junit.jupiter</groupId>
        <artifactId>junit-jupiter-engine</artifactId>
        <version>5.4.2</version>
        <scope>test</scope>
    </dependency>
</dependencies>

<build>
    <plugins>
        <plugin>
            <groupId>org.apache.maven.plugins</groupId>
            <artifactId>maven-surefire-plugin</artifactId>
            <version>2.22.1</version>
        </plugin>
    </plugins>
</build>
```

Når i kører <b>test</b>, så click test i <b>Maven Projects</b> -> <b>Lifecycle</b>
