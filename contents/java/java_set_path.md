
---

##### manual set path

- list

    - https://explainjava.com/java-path/#Setup_Java_Path_on_Windows_10
    - http://programmingloops.com/set-java-path-n-classpath-in-win-10/
    - https://www.java.com/zh_CN/download/help/path.xml

##### code

```cmd

setx CATALINA_HOME "C:\Tomcat 9.0";

setx MAVEN_HOME "D:\___App\apache-maven-3.6.0";

setx SPRING_HOME "D:\___App\spring-2.1.2.RELEASE";

setx Path "D:\___App\apache-maven-3.6.0\bin;D:\___App\spring-2.1.2.RELEASE\bin;%Path%";

```

---
end