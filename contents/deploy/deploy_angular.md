
---

#### deploy_angular_on_firebase_failed.md
- 2018-12-1
  - version: 6.1.1
  - wait google solved, "firebase login" still get Error.

---

#### deploy_angular_on_github_pages.md

- source guide
  - [https://github.com/angular-schule/angular-cli-ghpages](https://github.com/angular-schule/angular-cli-ghpages)

- other 
  - - https://coursetro.com/posts/code/64/How-to-Deploy-an-Angular-App-(Angular-4)

- install build and publish
     <!-- - > 使用当前lib, angular项目默认部署至, git Remotes中 Name="origin" 的远程仓库地址 -->
    
     - 0.0 must use terminal execute blow command...

     - 0 install lib
       - ```cmd
         npm i angular-cli-ghpages --save-dev
         ```
    
     - 1 add this to "package.json" -> "scripts"
       - ```cmd 
         "gh-bd": "ng b --aot --prod --base-href=https://org_name.github.io/repo_name/", 
         ```
       - ```cmd 
         "gh-pb": "npx ngh --dir=dist/local_project_name --no-silent ", 
         ```
         - --branch=master [optional]
            - --branch default: gh-pages
         - --no-silent [optional]
    
     - 2 check
       - Settings --> Github Pages
      
---

#### deploy angular on apache server

- https://angular.io/guide/deployment#routed-apps-must-fallback-to-indexhtml
    - https://ngmilk.rocks/2015/03/09/angularjs-html5-mode-or-pretty-urls-on-apache-using-htaccess/#thecode
    
        Apache: add a rewrite rule to the .htaccess file as shown :
        
        ```text
        RewriteEngine On
            # If an existing asset or directory is requested go to it as it is
            RewriteCond %{DOCUMENT_ROOT}%{REQUEST_URI} -f [OR]
            RewriteCond %{DOCUMENT_ROOT}%{REQUEST_URI} -d
            RewriteRule ^ - [L]
            # If the requested resource doesn't exist, use index.html
        RewriteRule ^ /index.html
        ```


---

#### deploy_angular_on_tomcat.md

- step
    - 0. https://javapointers.com/tutorial/creating-web-application-using-maven-in-intellij/
        - create a intellij idea maven-archetype-webapp project.
        - add angular app on webapp.

    - 1. add in /opt/tomcat/conf/context.xml
        ```xml
        <!-- REWRITE VALVE -->
        <Valve className="org.apache.catalina.valves.rewrite.RewriteValve" />
        <!-- // -->  
        ```

    - 2. add rewite.config file in specific project WEB-INF folder with below content such as 
         on /opt/tomcat/webapps/projectName/WEB-INF/rewrite.config
        ```config
        RewriteCond %{REQUEST_URI} !^.*\.(bmp|css|gif|htc|html?|ico|jpe?g|js|pdf|png|swf|txt|xml|svg|eot|woff|woff2|ttf|map)$
        RewriteRule ^(.*)$ /index.html [L]
        ```

- blog [it's working]
    - https://stackoverflow.com/questions/47366792/404-error-on-refresh-for-angularv4-deployed-on-tomcat-server
        - RouterModule.forRoot(routes, {useHash: true})
        - https://tomcat.apache.org/tomcat-8.0-doc/rewrite.html
    - https://stackoverflow.com/questions/51042875/url-rewriting-angular-4-on-tomcat-8-server
        - https://openguider.wordpress.com/angular-html5mode-in-tomcat-apache-8-5-4-gives-404-on-page-refresh/
        - http://tonyjunkes.com/blog/a-brief-look-at-the-rewrite-valve-in-tomcat-8/
    - https://stackoverflow.com/questions/39468479/angular-html5mode-in-tomcat-apache-8-5-4-gives-404-on-page-refresh
    - https://stackoverflow.com/questions/47366792/404-error-on-refresh-for-angularv4-deployed-on-tomcat-server/ [myabe]
    
- [useless]
    - https://stackoverflow.com/questions/41472774/deploy-angular2-app-to-tomcat8-routing-does-not-seems-to-work
    - http://www.thejavageek.com/2018/01/04/deploying-angular-app-tomcat/
    - http://code-adda.com/2018/05/deploy-angular-app-on-tomcat-server/

- [complexity]
    - https://dzone.com/articles/building-a-web-app-using-spring-boot-angular-6-and
        - https://techshard.com/2018/08/12/building-a-web-app-using-spring-boot-angular-6-and-maven/

---

#### spring boot spa

```java
@Controller
public class RouteController {
    @RequestMapping(value = "/{path:[^\\.]*}")
    public String redirect() {
        return "forward:/";
    }
}
```

- https://stackoverflow.com/questions/40769200/configure-spring-boot-for-spa-frontend
    - https://spring.io/guides/tutorials/spring-security-and-angular-js/
    - https://spring.io/blog/2015/05/13/modularizing-the-client-angular-js-and-spring-security-part-vii#using-ldquo-natural-rdquo-routes
    - https://github.com/spring-guides/tut-spring-security-and-angular-js/

---

#### dont know how to use

- list
    - http://csetutorials.com/deploy-angular-2-maven-webapp-on-tomcat.html

---
end
