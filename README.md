# SPYGAZER
Intra/Internetworked Information Gathering Toolset all within the comfort of your browser.

### What is SPYGAZER?

SPYGAZER (PeekingGlass Server) is an HTTP application layer (L7) webserver aimed at establishing an *informational collective dominion* over the current subnetwork in which it is configured/hosted.


### Built With:
* [Bottle](https://bottlepy.org/docs/dev/) - a lightweight WSGI micro web-framework used by the web application for path/request routing functionality.
    * *Web Server Gateway Interface* (WSGI) - standard specification (PEP 3333) upon which servers and python web applications/frameworks can communicate. Read more [here](https://peps.python.org/pep-3333/).
* [Bootstrap](https://getbootstrap.com/docs/5.3/getting-started/introduction/) - for the user-interface, files are hosted statically by SPYGAZER.
* `gevent`, `geventwebsocket` - for client-side request routing throughout the front-end (Bottle) web application server.
* Client-side Javascript for communicating with the python WSGI websocket server.
* Made with ❤️

## Documentation
The associated documentation will be available/produced as:
   * A `.pdf` (Portable Document File) and subsequently made accessible when the project is open sourced with a public release coming in version 1.0.0.
   * A Github markdown based "wiki" page. (*NOTE*: This will be posted shortly after the `.pdf` file is integrated into this public repository)
   * Each subsequent main route (i.e, /subshell, /dashboard) will have available help upon clicking the associated button.
      * This will include general documentation for the current page, and a listing breakdown of the functionality of said page.
      * Documentation for the entire SPYGAZER web application may be built into the server directory itself at a later point in time.

*Release?* (TBD)

## Preview

### > *Login Page*
![image](https://github.com/user-attachments/assets/2b353f92-04e2-4b08-9ffd-1c18919898e8)
<hr>

### > *Websocket Shell*

![image](https://github.com/user-attachments/assets/2ed0c99a-0d52-415b-ac29-76fabcdc8d49)


<h3><u>Websocket Shell Features:</u></h3>

1. Command execution on the fly.
1. In-built Python3 script manager (run, import).
1. Server wide shutdown capability.
1. Variable range text marking (highlighting).
   * Useful for color coding specific lines, characters or entire fields of text within the bounds of the console context.
1. Quick-access color customization options.
   * No need to access the navigation bar "Terminal Settings" in order to change color options. 
1. Command and UI based `clear` functionality.
   * Recursively delete the necessary child-elements to "reset" the screen origin back to default behavior.
      * *NOTE*: Default behavior = reloading the URI `/subshell`  
1. "Click-back" to console/terminal for responsive minimization of the navagation bar.
   * Allows both mobile and desktop operators to actively reposition the navbar when resuming console command invocations.
1. Back-end websocket server network status (ONLINE/OFFLINE) profiling detection.
1. Custom packet crafted Traceroute/ICMP facilities to extrapolate information pertaining to the functionality of the websocket server.

<hr>

### > *UPDATE: Support for in-built documentation*

![image](https://github.com/user-attachments/assets/a2b1d3a9-d683-4fd9-b61f-fa7e165064cc)

*Above Image: When testing in the latest release of the `Firefox` web browser.*

### > *Responsive Layout Positioning*
*NOTE*: Details displayed in regards to the phones virtual viewport boundary being set/emulated to that of a Samsung Galaxy S20 is irrelevant to the re-sizing/positioning ability that native Bootstrap elements have to offer. The bounds of each element will be scaled in accordance with the mobile devices unique physical layout itself.

![image](https://github.com/user-attachments/assets/f116f4a4-c53c-4538-8ebb-e7c645efd232)

![image](https://github.com/user-attachments/assets/37a13260-8a9d-41cc-9d8c-8a8a78baadfe)

![image](https://github.com/user-attachments/assets/787512cf-6b2f-4e9e-bb83-a08186c85d09)
