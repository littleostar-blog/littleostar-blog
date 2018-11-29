
---

#### _deploy_angular_app_on_github_pages
  - [https://github.com/angular-schule/angular-cli-ghpages](https://github.com/angular-schule/angular-cli-ghpages)
      
#### angular-cli-ghpages 安装 编译 并部署

 > 使用当前lib, angular项目默认部署至, git Remotes中 Name="origin" 的远程仓库地址


 - 0 安装
   - ```cmd
     npm i angular-cli-ghpages --save-dev
     ```
     - i -> install, 安装
     - --save-dev, 添加lib至package.json的同时. 执行npm install. 后面的-dev表示当前lib添加至开发模式依赖包列表
 
 
 - 1 编译并部署
   
   - ```cmd 
     ng b --aot --prod --base-href=https://组织名.github.io/存储仓库名/ && npx ngh --dir=dist/本地项目名 
     ```
     - b -> build, 编译
     - --aot, AOT编译
     - --prod, 生产模式
     - --base-href, 基础URL
     - --dir=dist/本地项目名, 针对angular6以后. 编译好的(即直接可部署的)项目存储在dist文件夹下
   
   or
   - ```cmd 
     "gh-bd": "ng b --aot --prod --base-href=https://组织名.github.io/存储仓库名/", 
     ```
   - ```cmd 
     "gh-pb": "npx ngh --dir=dist/本地项目名", 
     ```

 - 2 检查部署好的 github pages
   - Settings --> Github Pages
      
---

---

end
