# Sitefinity Boilerplate template & theme
An empty starting point for template & theme development based on HTML5Boilerplate & Modernizr compatible with Sitefinity's layout editor and Sitefinity Thunder.
This theme has no widget styling, but offers only a clean cross-browser normalized startingpoint, weighing only 3.9Kb without any extra markup.
Comes with 1 masterpage, 2 css files (normalize, layout) and pre-packed with minified production ready Modernizr.
  
Compatibility: Sitefinity `6.x`. HTML5Boilerplate `4.2.0`.
  

## Quick start
Copy the entire unzipped files inside your solutions /App_Data/WebsiteTemplates folder. Rename the folder to suit your needs.
Choose whether you want minified CSS, development CSS or .LESS files and publish your site.

### Manual installation
 - Log into Sitefinity backend. 
 - Choose Administration >> Settings >> Advanced >> Appearance >> Frontend themes
 - Select `Create new`.
 - Type in a userfriendly name.
 - Type in a path similar to `~/App_Data/Sitefinity/WebsiteTemplates/Boilerplate/App_Themes/Boilerplate`
 - Select `Save Changes`

 - Choose Design >> Page Templates
 - Select `Create a template`
 - Type in a userfriendly name.
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
 - Select the `Boilerplate` project and click `Upload`


## Features
* A Sitefinity optimized port of the HTML5 Boilerplate project (http://html5boilerplate.com).
* HTML5 ready, with ARIA role definition and fallback browser support through Modernizr
* Based on and compatible with the standard Sitefinity lay-out region editor.
* Cross browser CSS normalizations and vertical rhythm.
* Responsive design & mobile friendly with Sitefinity column support
* The latest jQuery via Sitefinity to ensure compatibility.
* Support for .LESS and .CSS.

### LESS vs CSS
Inside the App_Themes/Global directory you'll find 3 types of files, .less, .min.css and .css.
* The .min.css files are minified and production ready.
* The .css are development css files.
* The .less files are the .LESS versions with variables of the .css files.
If you're comfortable with .less, use it otherwise just delete them. If you don't need minified css, delete the .min.css files.

### Responsive design & Mobile friendly media-queries
Out of the box this theme & template are already responsive and mobile friendly. Inside the layout_transformations.css (or .less) you'll
find a print media-query already defined which is fully compatible with Sitefinity's layout editor.

### 1 column Masterpage
Inside the App_Master directory you'll find only 1 masterpage.
It is a HTML5 accessibility enhanced template based on 1 column layout, for easy alteration inside Sitefinity's layout editor. 
Header, nav, section and footer are defined with all the ARIA landmark roles. 
Complete with extra scriptwrapper placeholder which won't out on live sites so script & stylewidgets can be safely placed without breaking the PageEditor.

### Javascript & jQuery
jQuery is loaded from Sitefinity to ensure proper compatibility. Through Sitefinity settings, jQuery can be loaded locally or through CDN.
The masterpage references 2 .js files, script.top.min.js and script.bottom.min.js to seperate javascript loading.
The script.top.min.js already contains the latest minified Modernizr, script.bottom.min.js is empty and ready for your projects javascript/jQuery.

### Meta-data
Meta-tags are extracted into seperate MetaData.ascx to keep Masterpage clean and to allow for easier editing.
