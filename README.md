# OpenRehab Reference Project
This repository includes a landing page and all available web apps linked as submodules.

## Basic Installation
In a terminal, assuming you have git installed, type: 

```
$ git clone --recurse-submodules https://github.com/gmarzloff/OpenRehab.git
$ cd OpenRehab
$ python -m SimpleHTTPServer 8000
```
Then open the web app in a browser: http://localhost:8000

## View on Mobile device
While your SimpleHTTPServer is running, you can view the app on your phone or tablet, though this device must be connected to the same network as your computer (now webserver). First find out your computer's ip address. In OSX, you can run 

```
$ ifconfig | grep "inet " | grep -v 127.0.0.1 | cut -d\  -f2
```
In Windows, click Start -> Run -> cmd (enter)-> ipconfig (enter)

The address probably starts with 192.168.1.something. Type this address without the [ ] in your mobile browser: ```http://[ip address]:8000```

## More Details

1. The web apps use the [Framework7](https://framework7.io) library but it does not need to be downloaded from that link separately for OpenRehab to work. When you are ready to customize your web apps, we recommend you download it to see code examples and understand its features.

2. If you want to use this web app as a template for a customized version to your program, **fork** this repository first. 

3. This repository contains a landing page (index.html) that allows multiple OpenRehab web apps to run. You must run this in a web server, because the web apps make asynchronous requests. To start a web server, in a terminal, type ```cd OpenRehab```, run ```python -m SimpleHTTPServer 8000``` (or ```python -m http.server 8000``` for python 3) where 8000.  When you want to kill the server later, type Ctrl+C. There are many other server options to run this such as Apache, Node.js, and nginx. 

4. Open the web app in a browser: http://localhost:8000.

## Choosing Web Apps to include
Web apps are submodules in this repository. The current available options include:

  * Spinal Cord Injury (SCI)
  * Brain Injury (TBI)
  
 ### Add/Remove Link Buttons
 To do
 
 ### Add gitmodules
 To do
 
 ### Delete specific web apps
 If you want to remove a specific web app, you must delete its submodule references by running the following commands in a terminal ([source](https://davidwalsh.name/git-remove-submodule)).
 
