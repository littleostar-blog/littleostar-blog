
---

- pre setting

pom.xml
```xml
<project>
    <!--..-->
    <artifactId>springboot</artifactId>
    <packaging>war</packaging>
    
    <!--...-->
    <build>
        <finalName>${artifactId}</finalName>
        <plugins>
            <plugin>
                <groupId>org.springframework.boot</groupId>
                <artifactId>spring-boot-maven-plugin</artifactId>
            </plugin>
        </plugins>
    </build>
    
</project>
```

- intellij idea
    - spring boot demo
      - Maven Panel
        - choose your project
          - Lifecycle
            - package
    
    

---

end
