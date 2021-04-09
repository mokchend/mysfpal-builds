![alt text](http://url/to/img.png)

# MySFPal Application Builds
This app is a proof-of-concept more than anything else.

__Disclaimer__: 
I've worked on this application on my free/spare time since March 2021 and it's been a great experience turning my full stack development skills into action.
This app represent a reflection of my current thinking and is develop solely based on my own needs & requirements :-) 
The views expressed in this document are those of the author(s) and do not represent the views of Salesforce, nor other companies (directly or indirectly) associated with the author.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.

# Pre-Requisite
* [sfdx](https://developer.salesforce.com/tools/sfdxcli) - Working on it to remove this dependency !

# Introduction
MySFPal is your toolbox to interact with multiple Salesforce instance from a single application.
As a Salesforce Admin user, I have often use different tools & plugins to connect and interact with 
all my Salesforce instance (from development, integration,acceptance & production sandbox).

## Why this tools ?
* I wanted a single tool (no SFDX command line with their multitude of parameters, no Salesforce AppExchange, with nearly no installation & complex configurations) to easily repeat the same task over differents sandboxes in a simple and secured easy way.
*  I wanted to keep and maintain my full stack development skills while exploring new technologies & horizon
  
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
> The PHP Framework for Web Artisans (for the back end)
* [Node JS](https://nodejs.org/en/)
> Node.js® is a JavaScript runtime built on Chrome's V8 JavaScript engine.

Big thanks to thoses amazing products and the Open Source community!

__Note__: Combining thoses differents technologies into one single application is not an easy task, and I have spend days & nights troubleshooting thoses integrations.
However, it is so rewarding to see how this application helps me to optimize my time while working on Salesforce platform.

# Releases Notes
* Not released
