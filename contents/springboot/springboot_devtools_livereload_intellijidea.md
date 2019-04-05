
---

To solve this You can do like: 

- 1- Add LiveReload extension in your browser. (option)

- 2- Add devtools dependencies to your pom.xml
    - (if it's maven (spring-boot-devtools)). 

- 3- In your intellij IDEA go to: 
    - file->settings->build,execution,deployment. 
    - Go to ->compiler->build project automatically. 

- 4-In your intellij IDEA: 
    - SHIFT+Ctrl+A ->
        - registry-> 
            - compiler.automake.allow.when.app.running

---

```xml
        <dependency>
            <groupId>org.springframework.boot</groupId>
            <artifactId>spring-boot-devtools</artifactId>
            <scope>runtime</scope>
            <!--<optional>true</optional>-->
        </dependency>
        
```

---

- https://stackoverflow.com/questions/33869606/intellij-15-springboot-devtools-livereload-not-working
- https://medium.com/@codebyamir/work-faster-in-spring-boot-with-devtools-a74879272774

---
end