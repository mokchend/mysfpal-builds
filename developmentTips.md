
# Installation is extremely slow
* __TODO__ : Using electron-builder is slow due to the fact that I try to hack the installer by adding sfdx-cli node as an external dependency. This work great but the drawback is that installer took  11 mn to install a simple hello World application (and 5 mn to build it ?!) ?!
```
let fullPathCommandSfdx = is.dev()
  ? process.cwd() + `/node_modules/sfdx-cli/bin/run`
  : //: `${process.resourcesPath}/node_modules/sfdx-cli/bin/run`; // this is working except in build mode
    "`${process.resourcesPath}/tools/node_modules/sfdx-cli/bin/run`"; // work in build/installer mode
```
* Configuration vue.config.js
```
      builderOptions: {
        appId: "mysfpal-demo-builds-id",
        productName: "My Salesforce Pal Demo Builds",
        // Copy this folder outisde and above the asar file
        // https://github.com/nklayman/vue-cli-plugin-electron-builder/issues/1355
        extraResources: ["./tools"],

        asar: true,
```

# Packaging Issue
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
