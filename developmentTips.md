__Dev runtime:  yarn electron:serve__ : SFDX Command found => OK
```
[2021-05-08T13:36:51.673] [DEBUG] mysfpal - app.getAppPath(): C:\code\mysfpal-demo-builds\dist_electron
[2021-05-08T13:36:51.673] [DEBUG] mysfpal - __dirname: C:\code\mysfpal-demo-builds\dist_electron
[2021-05-08T13:36:51.673] [DEBUG] mysfpal - os.homedir(): C:\Users\cmok
[2021-05-08T13:36:51.673] [DEBUG] mysfpal - process.resourcesPath: C:\code\mysfpal-demo-builds\node_modules\electron\dist\resources
```

 __yarn electron:build__

Combinaison 1/ Unpacked : SFDX Command found => OK
& '.\dist_electron\win-unpacked\My Salesforce Pal Demo Builds.exe' 
```
"C:\code\mysfpal-demo-builds\dist_electron\win-unpacked\My Salesforce Pal Demo Builds.exe"
[2021-05-08T13:42:19.160] [DEBUG] mysfpal - app.getAppPath(): C:\code\mysfpal-demo-builds\dist_electron\win-unpacked\resources\app.asar
[2021-05-08T13:42:19.160] [DEBUG] mysfpal - __dirname: C:\code\mysfpal-demo-builds\dist_electron\win-unpacked\resources\app.asar
[2021-05-08T13:42:19.160] [DEBUG] mysfpal - os.homedir(): C:\Users\cmok
[2021-05-08T13:42:19.160] [DEBUG] mysfpal - process.resourcesPath: C:\code\mysfpal-demo-builds\dist_electron\win-unpacked\resources
```

Combinaison 2/ Setup Installation : SFDX Command found => KO
```
"C:\code\mysfpal-demo-builds\dist_electron\My Salesforce Pal Demo Builds Setup 0.1.0.exe"
[2021-05-08T13:45:56.477] [DEBUG] mysfpal - app.getAppPath(): C:\Users\cmok\AppData\Local\Programs\mysfpal-demo-builds\resources\app.asar
[2021-05-08T13:45:56.477] [DEBUG] mysfpal - __dirname: C:\Users\cmok\AppData\Local\Programs\mysfpal-demo-builds\resources\app.asar
[2021-05-08T13:45:56.477] [DEBUG] mysfpal - os.homedir(): C:\Users\cmok
[2021-05-08T13:45:56.477] [DEBUG] mysfpal - process.resourcesPath: C:\Users\cmok\AppData\Local\Programs\mysfpal-demo-builds\resources
```

Working in all context
```
let outputCmd = crossSyncExecutor(`${process.resourcesPath}/mysfdx.cmd`, [
  "force:auth:list",
  "--json",
]);
```
