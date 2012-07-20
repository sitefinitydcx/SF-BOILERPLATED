# Sitefinity 5 Twitter Bootstrap template and theme

A fully compatible port of the Twitter Bootstrap framework to be compatible with Sitefinity 5.


## Quick start

Copy the entire unzipped files inside your solutions /App_Data/WebsiteTemplates folder. 
Choose whether you want minified CSS, development CSS or .LESS files and publish your site.


## Features

* A Sitefinity optimized extension of the Twitter Bootstrap project (https://github.com/twitter/bootstrap/).
* HTML5 ready, with ARIA role definition and fallback browser support through Modernizr
* Compatible with Sitefinity's region editor
* Twitter Bootstrap is 'untouched' to allow for easy updating (NuGet/GitHub) or use with SASS port.


## LESS vs CSS

Inside the App_Themes/Global directory you'll find 3 types of files, .yui.less, .min.css and .css.
* The .min.css files are minified and production ready.
* The .css are development css files.
* The .yui.less files are the .LESS versions with variables of the .css files.
If you're comfortable with .less, use it otherwise just delete them. If you don't need minified css, delete the .min.css files.


## 1 Masterpage
Inside the App_Master directory you'll find only 1 masterpage.
It is a HTML5 accessibility enhanced template based on 1 column layout, for easy alteration inside Sitefinity's layout editor. 
Twitter Bootstrap's Navbar is included, section and footer are defined with all the ARIA landmark roles. 
Complete with extra scriptwrapper placeholder which won't out on live sites so script & stylewidgets can be safely placed without breaking the PageEditor.


## Javascript & jQuery
jQuery is loaded from CDN with local fallback option. The masterpage references seperate .js files, so you can easily remove bootstrap functionality you don't need.


## Sitefinity-icons
Included are all precomposed icons for the iPhone/iPad & Android devices, and Windows 8 pinning. 
The favicon.ico comes in 2 flavors. The default favicon.ico is 64x64 which is enhanced for IE9/IE10 sitepinning, an old 16x16 icon is included.


## Contributing
Credits are due where credits go and special thanks to @stevemcniven and @rollerboy1. For comments or questions use twitter @jbokkers


## License

### Major components:

* Twitter Bootstrap:  Apache License 2.0

### Everything else:

The Unlicense (aka: public domain)
