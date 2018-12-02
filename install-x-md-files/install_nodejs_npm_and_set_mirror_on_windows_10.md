#### on windows install nodejs yarn and set mirror

##### nodejs yarn, downlaod and install
- download
  - [node.js](https://nodejs.org/)
  - [yarn#windows-stable](https://yarnpkg.com/zh-Hans/docs/install#windows-stable)

##### set mirror
- Manage the npm configuration files

    https://docs.npmjs.com/cli/config
    
- npm
  - ```cmd
    npm config set registry https://registry.npm.taobao.org --global 
    ```

- yarn
  - ```cmd
    yarn config set registry https://registry.npm.taobao.org --global
    ```

##### test config

- ```cmd
  npm config list
  yarn config list
  ```

- ```cmd
  C:\WINDOWS\system32>npm config list
  ; cli configs
  metrics-registry = "https://registry.npm.taobao.org/"
  scope = ""
  user-agent = "npm/5.6.0 node/v8.11.3 win32 x64"

  ; globalconfig C:\Users\UserXXX\AppData\Roaming\npm\etc\npmrc
  registry = "https://registry.npm.taobao.org/"

  ; builtin config undefined
  prefix = "C:\\Users\\UserXXX\\AppData\\Roaming\\npm"

  ; node bin location = C:\Program Files\nodejs\node.exe
  ; cwd = C:\WINDOWS\system32
  ; HOME = C:\Users\UserXXX
  ; "npm config ls -l" to show all defaults.

  C:\WINDOWS\system32>
  ```
- ```cmd
  C:\Windows\system32>yarn config list
  yarn config v1.7.0
  info yarn config
  { 'version-tag-prefix': 'v',
    'version-git-tag': true,
    'version-commit-hooks': true,
    'version-git-sign': false,
    'version-git-message': 'v%s',
    'init-version': '1.0.0',
    'init-license': 'MIT',
    'save-prefix': '^',
    'bin-links': true,
    'ignore-scripts': false,
    'ignore-optional': false,
    registry: 'https://registry.npm.taobao.org',
    'strict-ssl': true,
    'user-agent': 'yarn/1.7.0 npm/? node/v8.11.3 win32 x64',
    lastUpdateCheck: 1530898202641 }
  info npm config
  {}
  Done in 0.12s.

  C:\Windows\system32>
  ```

##### mirror website url

> [mirror](https://npm.taobao.org/)

----------

end
