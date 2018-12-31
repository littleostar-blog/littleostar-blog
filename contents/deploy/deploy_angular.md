
---

- deploy_angular_on_firebase_failed.md
- 2018-12-1
  - version: 6.1.1
  - wait google solved, "firebase login" still get Error.

---

- deploy_angular_on_github_pages.md
- source guide
  - [https://github.com/angular-schule/angular-cli-ghpages](https://github.com/angular-schule/angular-cli-ghpages)

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

- deploy_angular_on_tomcat.md

- blog
    - https://stackoverflow.com/questions/47366792/404-error-on-refresh-for-angularv4-deployed-on-tomcat-server
        - RouterModule.forRoot(routes, {useHash: true})
        - https://tomcat.apache.org/tomcat-8.0-doc/rewrite.html [dont know how to do it]
    - https://stackoverflow.com/questions/41472774/deploy-angular2-app-to-tomcat8-routing-does-not-seems-to-work
    - https://stackoverflow.com/questions/51042875/url-rewriting-angular-4-on-tomcat-8-server
    
- [useless]
    - http://www.thejavageek.com/2018/01/04/deploying-angular-app-tomcat/
    - http://code-adda.com/2018/05/deploy-angular-app-on-tomcat-server/

---

- https://coursetro.com/posts/code/64/How-to-Deploy-an-Angular-App-(Angular-4)

- dont use
- http://csetutorials.com/deploy-angular-2-maven-webapp-on-tomcat.html

---
end
