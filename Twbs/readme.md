# Sitefinity Twitter Bootstrap template and theme
A full port of the Twitter Bootstrap 3 framework to be compatible with Sitefinity 6. 
Empty and optimized starting point which is fully Bootstrap Responsive and Sitefinity mobile compatible.
  
Compatibility: Sitefinity `6.x`. Twitter Bootstrap `3.0.0`.
  

## Quick start
Copy the entire unzipped files inside your solutions /App_Data/WebsiteTemplates folder. Rename the folder to suit your needs.
Choose whether you want minified CSS, development CSS or .LESS files and publish your site.

### Manual installation
 - Log into Sitefinity backend. 
 - Choose Administration >> Settings >> Advanced >> Appearance >> Frontend themes
 - Select `Create new`.
 - Type in a user-friendly name.
 - Type in a path similar to `~/App_Data/Sitefinity/WebsiteTemplates/Boilerplate/App_Themes/Twbs`
 - Select `Save Changes`

 - Choose Design >> Page Templates
 - Select `Create a template`
 - Type in a user-friendly name.
 - Select `Use template`
 - Select `Select another Template`
 - Select `Use your own .master file`
 - Select `Browse other folders` and locate the .Master in your folder structure.
 - Select `Use selected` and `Create and go to add content`.

 - On the template editor screen choose `Theme` on the top right part of the screen.
 - Select `Boilerplate` from the dropdown to apply our theme to our template.

### Automatic installation with Thunder
 - Ensure a valid connection to your Sitefinity installation exists.
 - Open the Sitefinity Explorer in VisualStudio.
 - Right click `Website Templates` and select `Upload Website Template`.
 - Select the `Twbs` project and click `Upload`


## Features
* A Sitefinity optimized extension of the Twitter Bootstrap project (https://github.com/twbs/bootstrap/).
* Includes Kendo UI Web and Kendo UI Bootstrap theme with LESS support
* HTML5 ready, with ARIA role definition and fall back browser support through Modernizr and Respond.js
* Compatible with Sitefinity's region editor
* Additional layout widgets included for Twitter Bootstrap 3
* Twitter Bootstrap is 'untouched' to allow for easy updating (NuGet/GitHub) or use with SASS port.

### LESS vs CSS
Inside the App_Themes/Global directory you'll find 3 types of files, .less, .min.css and .css.
* The .min.css files are minified and production ready.
* The .css are development css files.
* The .less files are the .LESS versions with variables of the .css files.
If you're comfortable with .less, use it otherwise just delete them. If you don't need minified css, delete the .min.css files.

### 1 Masterpage
Inside the App_Master directory you'll find only 1 masterpage.
It is a HTML5 accessibility enhanced template based on 1 column layout, for easy alteration inside Sitefinity's layout editor. 
Twitter Bootstrap's regions are included, section and footer are defined with all the ARIA landmark roles. 
Complete with extra scriptwrapper placeholder which won't output on live sites so script & stylewidgets can be safely placed without breaking the PageEditor.

### KendoUI
Kendo UI Web is now included by default and loaded from Sitefinity Resource to ensure proper compatibility.
If you don't need/want Kendo UI remove script reference from .Masterpage and remove the KendoUI region from sfnormalize.less (or css file). 

### Javascript & jQuery
jQuery is loaded from Sitefinity resource to ensure proper compatibility. 
The masterpage references 2 .js files, script.top.min.js and script.bottom.min.js to separate javascript loading.
The script.top.min.js already contains the latest minified Modernizr, script.bottom.min.js is empty and ready for your projects javascript/jQuery.

### Meta-data
Meta-tags are extracted into separate MetaData.ascx to keep Masterpage clean and to allow for easier editing.

## Sitefinity-icons
Included are all precomposed icons for the iPhone/iPad & Android devices, and Windows 8 pinning. 
The favicon.ico comes in 2 flavors. The default favicon.ico is 64x64 which is enhanced for IE9/IE10 sitepinning, an old 16x16 icon is included.

## Layout widgets
7 Default Twitter Bootstrap layout regions/widgets, including sample ToolboxesConfig.config can be found here (https://github.com/jbokkers/SF-BOILERPLATED/tree/master/LayoutControls)
