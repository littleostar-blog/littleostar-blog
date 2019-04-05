- source
    - https://github.com/meteor/docs/blob/version-NEXT/long-form/alternate-windows-installation.md

---

##### 1 rar software
  
  - 
    - [7z](https://www.7-zip.org/)
    - [winrar](https://rarlab.com/download.htm)
  
##### 2 downlaod meteor offline install zip

  - [meteor latest zip](https://packages.meteor.com/bootstrap-link?arch=os.windows.x86_32)

##### 3 check meteor target

  - use the cmd to find
    - ```cmd
      echo %LocalAppData%\.meteor
      ```
  
  - the show like this
    - ```cmd
      C:\WINDOWS\system32>echo %LocalAppData%\.meteor
      C:\Users\UserName\AppData\Local\.meteor
      ```
  

##### 4 unzip the latest zip to target
  

##### 5 add .meteor to PATH

  - ```cmd
    C:\Users\UserName\AppData\Local\.meteor
    ```

##### 6 test meteor command

  - ```cmd
    C:\WINDOWS\system32>meteor
    run: You're not in a Meteor project directory.

    To create a new Meteor project:
      meteor create <project name>
    For example:
      meteor create myapp

    For more help, see 'meteor --help'.
    ```

---

end
