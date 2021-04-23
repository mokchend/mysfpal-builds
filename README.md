> No thank you, we're too busy... 
> We are too busy for a more efficient and user friendly solution.
> 
> #KISS #innovation #fullstack #technology #fun

![No Thanks, We are too busy ...](https://github.com/mokchend/mysfpal-builds/blob/main/WeAreTooBusy.png)

# MySFPal Application Builds
This application is a proof-of-concept more than anything else (Some functionnalities are still work in progress until I really need it)
The version 1.0.0 should represent a stable (& usable) version, with all tests validated and require no dependencies to be installed.

__Disclaimer__: 
I've worked on this application on my free/spare time since March 2021 and it has been a great experience turning my full stack development skills into action.
This app represent a reflection of my current thinking and is develop solely based on my own needs & requirements :-) 
The views expressed in this document are those of the author(s) and do not represent the views of Salesforce, nor other companies (directly or indirectly) associated with the author.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.


# Audience
This tools can target the following role in Salesforce Community:
- Business or Technical consultant
- Business Architect
- System Administrator
- Technical/Program Architect
- Technical Account Manager
 
# Functionnalities / Completion percentage
- Password less sandboxes connexion (but as secure as sfdx command line) - 100%
- Common Task automation (Metabackups & Analysis) - WIP 50%
- DB Replicator - SQLite DB support to extend SOQL limitation by using real SQL joins for quick org metric analysis - WIP 90%
- UML Schema Browser - WIP 90%
- Role/Group Hierarchy Browser - WIP 60%
- SObject & SOQL Plus - WIP 80%
- Recent List of Metadata Changes - 100%
- Metadatas & records dependencies - WIP 80%
- Neo4J Integration - WIP 50%
- Copado US dependencies analyzer - WIP 80%

# Pre-Requisite
* No dependencies, just an executable and you are good to go !
* Salesforce System Admin (or equivalent) profile to access your Salesforce sandboxes


# Introduction
MySFPal is your toolbox to manage multiple Salesforce instance from a single & multi-platform application.
As a Salesforce Admin user, I have often use different tools & plugins to connect and manage 
all my Salesforce instance (from development, integration,acceptance & production sandbox).
I want a tools that is simple & easy to use (#KISS) and do not require libraries, languages or command line dependencies to be installed on my computer. 



## Why this tools ?
* I wanted a single tool (no SFDX command line with their multitude of parameters, no Salesforce AppExchange, with nearly no installation & complex configurations) to easily repeat the same task over differents sandboxes in a simple and secured easy way.
*  As a hobbyist developper, I wanted to keep and maintain my full stack development skills while exploring new technologies & horizons
  
## How ?
A cross platform Multi Page Application to interact with your multiple Salesforce instance.
A simple executable that work on Windows/Mac (to be tested) and rely on your current SFDX configuration

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
> The PHP Framework for Web Artisans (for future back end implementation)
* [Node JS](https://nodejs.org/en/)
> Node.js® is a JavaScript runtime built on Chrome's V8 JavaScript engine.
* [SQLite 3](https://www.sqlite.org/)
> SQLite is a C-language library that implements a small, fast, self-contained, high-reliability, full-featured, SQL database engine. 

Big thanks to thoses amazing products and the Open Source community!

__Note__: Combining thoses differents technologies into one single application is not an easy task, and I have long nights, spend days & weekends troubleshooting thoses integrations. However, it is so rewarding to see how this application helps me to optimize my time and become more efficient while working on Salesforce platform.


 
# Releases
* Not Released Yet
