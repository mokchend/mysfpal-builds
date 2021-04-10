# Change Logs
* v0.8.4 2021-04-10
  * Add EventBus globally to the app for sibling components communication
  * Add logged header to each components to let the user know which is the current Salesforce alias he/she working on 
  * Building add alias for Windows only (TODO: need to handle the spawn process differently on Linux & Mac OS system)

* v0.8.3 2021-04-09
  * Add Logger file from ipcMain & ipcRenderer process
  * Support application configuration file
  * Synchronize the selected alias (fro mElectron) with the properties config to be reused with gulp tasks
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
  
