# OpenRehab Reference Project
This repository includes a landing page and all available web apps linked as submodules

1. This web app uses the [Framework7](https://framework7.io) library but does not need to be installed to run this webapp. It is recommended that you download it to see code examples and understand its features.

2. If you want to use this web app as a template for a customized version to your program, **fork** this repository first. 

3. This repository contains a landing page (index.html) that allows multiple OpenRehab web apps to run. You must run this in a web server, because the web apps make asynchronous requests. To start a web server, in a terminal, type ```cd /[Your/Folder/Path]/SCIM-Rotation-Guide```, run ```python -m SimpleHTTPServer 8000``` (or ```python -m http.server 8000``` for python 3) where 8000.  When you want to kill the server later, type Ctrl+C. There are many other server options to run this such as Apache, Node.js, and nginx. 

4. Open the web app in a browser: http://localhost:8000.

## Choosing Web Apps to include
Web apps are submodules in this repository. The current available options include:

  * Spinal Cord Injury (SCI)
  * Brain Injury (TBI)
  
 ### Add/Remove Link Buttons
 To do
 
 ### Add gitmodules
 
 ### Delete specific web apps
 If you want to remove a specific web app, you must delete its submodule references by running the following commands in a terminal ([source](https://davidwalsh.name/git-remove-submodule)).
 
