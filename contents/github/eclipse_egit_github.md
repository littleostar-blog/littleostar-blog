
---

- https://wiki.eclipse.org/EGit/User_Guide#Push_Upstream
    - https://help.github.com/articles/working-with-ssh-key-passphrases/
    - https://github.com/settings/keys
    - demo: https://github.com/littleostar-java/say-hello

#### Create Repository

##### 1
- Create a new Java project HelloWorld. (In this case, the project was built outside of your Eclipse Workspace.)

##### 2
- Select the project, click File > Team > Share Project.
- Select repository type Git and click Next.

##### 3
- To configure the Git repository select the new project HelloWorld.

##### 4
- Click Create Repository to initialize a new Git repository for the HelloWorld project. 
  If your project already resides in the working tree of an existing Git repository the repository is chosen automatically.

##### 5 
- Click Finish to close the wizard.
- The decorator text "[master]" behind the project shows that this project is tracked in a repository on the master branch and the question mark decorators show that the .classpath and .project and the .settings files are not yet under version control.

---

#### Track Changes

##### 1

- Click Team > Add to Index on the project node. (This menu item is named Add on older versions of Egit.)
- The + decorators show that now the project's files have been added to version control.
- Mark the "bin" folder as "ignored by Git", either by right-clicking on it and selecting Team > Ignore or by creating a file .gitignore in the project folder with the following content:
```cmd
/bin
```
- This excludes the bin folder from Git's list of tracked files.
- Add .gitignore to version control (Team > Add):

##### 2
- You may have to set your Package Explorer filters in order to see .gitignore displayed in the Package Explorer. To access filters, select the down arrow on the right edge of the Package Explorer tab to display View Menu.

---
end
