# Change Logs
* v0.9.6 2021-05-09
  * Refactor & modularize code (log4j, sfdx command executor)
  * Optimize call to open an URL without using calling sfdx
  * Document usage/use case based on feedbacks from CSG collegue 
  * Add support to monitor Scratch & Non ScratchOrg
  * ASAR packaging is finally working: use the builderOptions.extraResources to package the needed assets outside the ASAR file
  * Adding sfdx-cli version in the LoggedAs component
  * Remove npm sfdx-cli dependancy as production build not able to call this command line. Workaround is to try auto-discover the SFDX installation. Advantage is that Build size reduce from 50Mb. __TO_BE_IMPROVED__ 


* v0.9.5 2021-05-06
  * Ubuntu, Mac OSX, Windows VM to handle the build the factory - __TODO__ : trigger a WebHook to build on code commit, check how to bundle Linux build
  * Support a clean (e.g no sfdx aliases defined) in your OS, Hide Menu Item when no alias defined
  * Add support Development Build versus Production Build - __TODO__ : pluginOptions.electronBuilder.builderOptions.asar = false : not recommended build, but having issue to use program defined in node_modules when use ASAR bundle. Drawback is that build process is slower but solve the needs to have sfdx ou gulp installed by the end user.
  (asar usage is disabled — this is strongly not recommended  solution=enable asar and use asarUnpack to unpack files that must be externally available)
  * Refactor the way sfdx commands are called as behavior from Development or Production Build are not working the same way (differents path execution). Needs to complexify the code to handle this situation. __TODO__ : Find a better way to implement it
  * Automatic application update when publishing a new version
  * Centralized log, improve error handling (a virgin OS: Mac & Windows) to catch/trap unhandled errors
  * Update About vue form to display if we are in Development or Production Build.
  * __WARNING__: Move local files/backups/workspace zone to __$HOME/data01__, consistent location on ALL OS : __$HOME/mysfpal.log__ and __$HOME/mysfpal-config.json__ to avoid zero configuration from the end user and ease the integration (__TODO__: Rework on C:\Users\cmok\AppData\Roaming\MySFPal\config.json)
  * 

* v0.9.4 2021-05-02
  * Build Ubuntu & Mac OSX VM to generate builds for theses OS
  * Build scripts for Ubuntu Linux and Mac OSX - 64 bits
  * Better Error handling when alias do not exist on a brand new OS
  * All data01 folder and mysfpal-config.json now reside in the home directory of the user to allow OS portability

* v0.9.3 2021-04-26
  * Passwordless SOAP support
  * Build Sample code calling SOAP Web Methods: login, findDuplicates, findDuplicatesByIds, query

* v0.9.3 2021-04-24
  * __WIP__: Adding SOAP support
  * __WIP__: Full Metadata Backups, Full Profile & permission set extraction
  * __WIP__: Daily Auto-schedule Metdata Backup from a configurable configuration

* v0.9.2 2021-04-21
  * Adding log4j support to capture debugs / error message for a better troubleshooting. 
  * __TODO__ : Remove all console.log / console.dir in the code 
  * Improve Gulp tasks (SOQL2DB) call from Main Process
  * Windows limitation when SOQL query is larger than 255 characteres (The command line is too long).
  * __TODO__ : Using SQLite from the main Process generate "uncaughtException:Please install sqlite3 package manually"
  * Dynamic DB Bulk Insert - support JSON result and compound fields
  * EventLog File download
  * Add jsforce Api version support: update globally the json config when alias is selected 
  * __TODO__ : Synch sfdx apiVersion and jsforce apiVersion to have a consistent experience & results
  * __TODO__ : Improve Gulp Task to signal the end of the task to the main process 
  * __TODO__ : Datatypes in sqlite3 are varchar/string only + JSON - Can be improved to mapped the right data types from SF Sobject metadatas

* v0.9.1 2021-04-18
  * Adding support gulp 4 tasks with parameters using minimist
  * Refactor application properties to better structure the default application configuration
  * Synchronize the GUI Alias selection with application properties via store.onDidChange event handler
  * Remove the global/system/OS sfdx & gulp dependencies
  * When no alias exist (or defined in your system), the application fail to run. Instead, display a message to the user to register an alias and hide the pane "Alias Selector" & "Navigate To".
  * __WIP__:Adding build support for linux/mac OS

* v0.9.0 2021-04-16
  * Adding Bulk Query support
  * Adding toaster notification functionnalities
  * __TODO__: Rebuild the Monitor Bulk Data Load Jobs to allow minimal user action to download the batch results or errors
  * __TODO__: Exporting SOQL query to a local sqlite2 database to avoid SOQL query limitation (compound field not supported with simple aggregation)
  
* v0.8.6 2021-04-13
  * Adding Spinner when executing SOQL Query
  * Adding horizontal MultiPane to separate the SOQL Query Editor & allow to scroll dynamic table results without hiding the query

* v0.8.5 2021-04-12
  * Standard table result with simple error handling
  * __TODO__: [Capture the release stats in app itself](https://tooomm.github.io/github-release-stats/?username=mokchend&repository=mysfpal-builds)
  * Refactor & Componentized the SObjectPlus page
  * Redesign the developer workflow experience with SOQL Query : Seach SObject/ SOQL Query / Search by Field Name
  * Adding Fuzzing Search component and implement it on SObjectPlus __TODO__: (this is a prototype, but does the job)

* v0.8.5 2021-04-11
  * __TODO__: need ability to remove an alias ?
  * Add toaster message
  * Add SOQL Query editor functionnality

* v0.8.4 2021-04-10
  * Add EventBus globally to the app for sibling components communication
  * Add logged header to each components to let the user know which is the current Salesforce alias he/she working on 
  * Building add alias for Windows only (TODO: need to handle the spawn process differently on Linux & Mac OS system)

* v0.8.3 2021-04-09
  * Add Logger file from ipcMain & ipcRenderer process
  * Support application configuration file
  * Synchronize the selected alias (from Electron) with the properties config to be reused with gulp tasks
  * Update the Cockpit page to handle alias usage (add/search/delete/navigate) and add WIP for others tab

* v0.8.2 2021-04-07
  * Musing: Network grappes of records

* v0.8.0 2021-04-05
  * hack: Execute a gulp task from renderer process, retrieve the result and display it on the screen. There should be a better way to implement this.

* v0.7.2 2021-04-02
  * Add in-memory scheduler support
  * Auto refresh current session and keep it alive
  * Gulp Task execution & output redirected in the renderer process

* v0.7.1: 2021-03-31
  * Adding PlantUML generation for lookup relation

* v0.6.1: 2021-03-28
  * Adding Code Coverage Stats

* v0.5.1: 2021-03-27
  * Add Graphviz support

* v0.4.1: 2021-03-26
  * Adding code editor support

* v0.3.1: 2021-03-21
  * Add modal About Window

* v0.3.0: 2021-03-21
  * Clean Menu
  * Use RouterView and Dynamic Component
  * Alias Selector - WIP
  * SObject Plus - WIP

* v0.2.1: 2021-03-14
  * Adding contextMenu 
  
* v0.2.1: 2021-03-14
  * About page store in public folder - NOT Working once package for production - TODO
  * Global nav bar & footer page + future applications ideas to build
  * Support Single and Multiple page application using vue router
  * Script to publish windows 64 bits releases on GitHub
  * Icon creation
  
