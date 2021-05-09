> No thank you, we're too busy... 
> We are too busy for a more efficient and user friendly solution to deal with Salesforce sandboxes.
> 
> #kiss #innovation #fullstack #technology #Salesforce #fun

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

# Introduction
MySFPal is your toolbox to administer multiple Salesforce instance from a single & multi-platform application.
As a Salesforce Admin user, I have often use different tools & plugins to connect and manage  all my Salesforce 
instance (from development, integration,acceptance & production sandbox).
I want a tool that is simple & easy to use (#KISS) and do not require external libraries/language, any command line dependencies 
or any App Exchange to be installed or configured. 

# Audience
This tools can target the following role in __Salesforce Community__:
- Business consultant or Business Architect
- Developper / System Administrator
- Technical/Program Architect / Technical Account Manager
-
 
# Functionnalities / Completion percentage
- List all aliases created by your SDFX command line and display usefull information - 100%
- Password less sandboxes connexion (but as secure as sfdx command line on your computer) - 100%
- Most used link access in one click - 100%
- Recent List of Metadata Changes - 100%
- On-Demand SQLite DB Replicator support: extend SOQL limitation by using real SQL joins for quick data analysis & discovery (3.8M records in 35mn) - WIP 90%
- Plant UML Schema Browser integration - WIP 90%
- GraphViz Schema integration - WIP 90%
- Copado US dependencies analyzer (require NEO4J instance) - WIP 80%
- Metadatas & records dependencies - WIP 80%
- SObject & SOQL Plus Explorer - WIP 70%
- Role/Group Hierarchy Browser - WIP 60%
- Common Task automation (Metabackups & Analysis) - WIP 50%
- Neo4J Integration - WIP 50%
- MetaData Backups & Org info / limits gathering scheduler - WIP 50%
- Mass Download Event Logs - WIP 50%
- Mass Download & Analyze Debugs Logs - WIP 50%
- Mass Download Bulks Jobs request & results - WIP 50%
- Setup Audit Trail Plus - WIP 50%
- Auto upgrade application - WIP 50%

# Pre-Requisite
* No dependencies, just an executable and you are good to go !
* Salesforce System Admin (or equivalent) profile to access your Salesforce sandboxes

## Why this tools ?
* I wanted a single tool (no SFDX command line with their multitude of parameters, no Salesforce AppExchange, with nearly no installation & complex configurations) to easily repeat the same task over differents sandboxes in a simple and secured easy way.
* As a hobbyist developper, I wanted to keep and maintain my full stack development skills while exploring new technologies & horizons
  
## What ?
A cross-platform Multi Page Application to interact with your multiple Salesforce instance.
A simple electron executable that work on Windows/Mac/Linux (to be build & tested) that rely on your current SFDX configuration

## How ?
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

__Note__: Combining thoses differents technologies into one single application is not an easy task, and I have spent long nights, workation days & weekends troubleshooting thoses integrations. However, it is so rewarding to see how this application helps me to optimize my time and become more efficient & productive while working on Salesforce platform.
 
# Releases
* Not Released Yet
