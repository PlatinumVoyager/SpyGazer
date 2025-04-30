# SPYGAZER

[![PlatinumVoyager - SpyGazer](https://img.shields.io/static/v1?label=PlatinumVoyager&message=SpyGazer&color=blue&logo=github)](https://github.com/PlatinumVoyager/SpyGazer "Go to GitHub repo")
[![stars - SpyGazer](https://img.shields.io/github/stars/PlatinumVoyager/SpyGazer?style=social)](https://github.com/PlatinumVoyager/SpyGazer)
[![forks - SpyGazer](https://img.shields.io/github/forks/PlatinumVoyager/SpyGazer?style=social)](https://github.com/PlatinumVoyager/SpyGazer)
[![License](https://img.shields.io/badge/License-The_Unlicense-blue)](https://github.com/PlatinumVoyager/SpyGazer/blob/main/LICENSE)

> [!NOTE]
> This project is undergoing active development. There is no official release date as of now. Stand by.

### <ins>What is SPYGAZER?</ins>

SPYGAZER (PeekingGlass Server) is an HTTP application layer (L7) webserver aimed at establishing an *informational collective dominion* over the current subnetwork in which it is configured/hosted.
* *Informational Collective Dominion* - the substratum in which SPYGAZER operates is as follows: Have a "spyglass view" of the current network in which the PeekingGlass HTTP TCP/IP server has been established.
‎
### <ins>Built With</ins>
* [Bottle](https://bottlepy.org/docs/dev/) - a lightweight WSGI micro web-framework used by the web application for path/request routing functionality.
    * *Web Server Gateway Interface* (WSGI) - standard specification (PEP 3333) upon which servers and python web applications/frameworks can communicate. Read more [here](https://peps.python.org/pep-3333/).
 
* [Bootstrap](https://getbootstrap.com/docs/5.3/getting-started/introduction/) - for the user-interface, files are hosted statically by SPYGAZER.
* `gevent`, `geventwebsocket` - for server-side request routing throughout the front-end (Bottle) web application server.
‎
* Client-side Javascript for communicating with the python WSGI websocket server.
* Made with ❤️

### <ins>Release?</ins> 
*To be determined.*

## Documentation
The associated documentation will be available/produced as:
   * A `.pdf` (Portable Document File) file subsequently made accessible when the project is open sourced with a public release coming in version 1.0.0.
   * A Github markdown based "wiki" page. (*NOTE*: This will be posted shortly after the `.pdf` file is integrated into this public repository)
     
   * Each subsequent main route (i.e, /spygazer/subshell, /spygazer/dashboard) will have available help upon clicking the associated button.
      * This will include general documentation for the current page, and a listing breakdown of the functionality of said page.
      * Documentation for the entire SPYGAZER web application may be built into the server directory itself at a later point in time.
<br>

## Graphical User Interface Preview
> [!WARNING]
> *All images depicted are a work-in progress and are not final.*

### > <ins>*Login Page*</ins>
The SPYGAZER authentication portal (login page) has a purposefully sleek and generic graphical interface. 
<br>
* Features a "blacked out" form entry feature that disables the viewing of ANY characters, input, etc.
<br>

![image](https://github.com/user-attachments/assets/2b353f92-04e2-4b08-9ffd-1c18919898e8)
<hr>

### > <ins>*Main Dashboard*</ins> (work-in progress)
* Live animated background.
* Real-time server updates within the dashboard viewport panel.
  
![image](https://github.com/user-attachments/assets/b2771d58-8162-4ecb-8e4c-cb13eecc4d8b)

### > <ins>*Process Manager*</ins> (OLD UI Mockup)
  
![image](https://github.com/user-attachments/assets/916ed5ac-c2cb-47d0-b117-9ee91b8bd707)

### > <ins>*Process Manager*</ins> (Dashboard Integration OLD)
![image](https://github.com/user-attachments/assets/d261348e-bc14-46cc-ae02-ded6d60dcc7b)

### > <ins>*Process Manager*</ins> (Dashboard Integration NEW)
![image](https://github.com/user-attachments/assets/10d09a3e-f18c-4148-9f6b-005027350fc0)
![image](https://github.com/user-attachments/assets/fb3938fa-3482-4a21-8138-4fbcfb8d4c60)
![image](https://github.com/user-attachments/assets/6528c9ea-49e3-41ef-8086-b233e1eca3dd)
![image](https://github.com/user-attachments/assets/1ddef8b2-05a4-41db-b0e2-e426609fa76d)
![image](https://github.com/user-attachments/assets/c4966bc7-4e92-44ec-9bfb-e6dffed55902)

* Added the ability to search through processes for information which concerns the following:
   * Name of the process.
   * Status of the process: *Running*, *Sleeping*, *Idle*. (ALL supported process state types can be seen in the image below)
      * ![image](https://github.com/user-attachments/assets/a0f96036-e237-4401-bdd5-a6526f37cbc5)
   * Process states can be filtered with the click of a button via the "Process Stats" dropdown menu within the Process Managers sub-window context.
   * ANY/* other text that is contained within the bounds of the process container.
         
<hr>

### > <ins>*Websocket Shell*</ins> (work-in progress)
* Support for CSS (*Cascading Style Sheets*) font-family and font-size custom user defined declarations via JavaScript DOM manipulation will come before release.
  
![image](https://github.com/user-attachments/assets/3011dc6e-1d3b-4737-a063-6586e38259ee)

### > <ins>*Responsive Layout Positioning*</ins> (Mobile Operators)
> [!NOTE]
> For remote clients using a mobile device, custom JavaScript and CSS styling has been built into the application beyond that of the original bootstrap base functionality. This will correctly position elements justly to accomodate for a narrower virtual viewport.

![image](https://github.com/user-attachments/assets/9637b932-6d88-4fb9-90e7-cb0c86c3b693)

![image](https://github.com/user-attachments/assets/f9de5143-2528-4f95-afe1-92ed09f9ba44)
* `psutli_test.py` - Totally not a typo ;)

<h3><ins>Websocket Shell Features</ins></h3>

1. Command execution on the fly.
1. In-built Python3 script manager (run, import).
   * ![image](https://github.com/user-attachments/assets/b9afba97-8330-48c6-b89e-649485021f61)
    
1. Server wide shutdown capability (*must provide server shutdown key*).
   
   ![image](https://github.com/user-attachments/assets/524898fc-93b7-447a-b25a-f6f74f51f9b6)

1. Variable range text marking (highlighting).
   * Useful for color coding specific lines, characters or entire fields of text within the bounds of the console context.
1. Quick-access color customization options.
   * No need to access the navigation bar "Terminal Settings" in order to change color options. 
1. Command and UI based `clear` functionality.
   * Recursively delete the necessary child-elements to "reset" the screen origin back to default behavior.
      * *NOTE*: Default behavior = reloading the URI `/spygazer/subshell`  
1. "Click-back" to console/terminal for responsive minimization of the navagation bar.
   * Allows both mobile and desktop operators to actively reposition the navbar when resuming console command invocations.
1. Back-end websocket server network status (ONLINE/OFFLINE) profiling detection.
1. Custom packet crafted Traceroute/ICMP facilities to extrapolate information pertaining to the functionality of the websocket server.

<hr>

### > <ins>*Support for in-built documentation*</ins>

![image](https://github.com/user-attachments/assets/a2b1d3a9-d683-4fd9-b61f-fa7e165064cc)

*Above Image: When testing in the latest release of the `Firefox` web browser.*
