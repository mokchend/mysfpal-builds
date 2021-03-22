# MySFPal Application Builds
This app is a proof-of-concept more than anything else. 
__Disclaimer__: This app is develop solely based on my own need & based on the repetitive taks. 

# Introduction
MySFPal is your toolbox to interact with multiple Salesforce instance from a single application.
As a Salesforce Admin user, I have often use different tools & plugins to connect and interact with 
all my customer instance (from development, integration,acceptance & production sandbox).

## Why ?
I wanted a tool to easily repeat the same task over differents sandbox in a simple and easy way without 
the hassle to provide credentials or remember the multitude parameters to provide to the SFDX command line. 

## How ?
A cross platform Multi Page Application to integract with your multiple Salesforce instance.

## What ?
This tool is heavily relying on the following technologies :
* [sfdx](https://developer.salesforce.com/tools/sfdxcli)
> Single command-line interface for Force.com and all Salesforce DX features
* [jsForce](https://jsforce.github.io/)
> Develop Salesforce apps with JavaScript, whether it's running on server or web browser. 
* [Gulp Tasks](https://gulpjs.com/) 
> A toolkit to automate & enhance your workflow
* [Vue JS](https://vuejs.org/) 
> The Progressive JavaScript Framework
* [Salesforce Lightning Design System](https://www.lightningdesignsystem.com/) 
> Create the World’s Best Enterprise App Experiences
* [Electron JS](https://vuejs.org/)
> Build cross-platform desktop apps with JavaScript, HTML, and CSS
* [Taildwindcss](https://tailwindcss.com/)
> Rapidly build modern websites without ever leaving your HTML.
* [Laravel](https://laravel.com/)
> The PHP Framework for Web Artisans (for the back end)
* [Node JS](https://nodejs.org/en/)
> Node.js® is a JavaScript runtime built on Chrome's V8 JavaScript engine.

Big thanks to thoses amazing products and the Open Source community!
__Note__: Combining thoses differents technologies into one single application is not an easy task. But  I really enjoyed working on this application 
during my week-end & spare time. And how it is rewarding to see this application helping me to optimize
my time while working on Salesforce.

# Releases Notes
* Not released

# Change Logs
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
  
