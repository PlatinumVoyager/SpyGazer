# SPYGAZER
Intra/Internetworked Information Gathering Toolset all within the comfort of your browser.

### What is SPYGAZER?

SPYGAZER (PeekingGlass Server) is an HTTP application layer (L7) webserver aimed at establishing an *informational collective dominion* over the current subnetwork in which it is configured/hosted.


### Built With:
* [Bottle](https://bottlepy.org/docs/dev/) - a lightweight WSGI micro web-framework used by the web application for path/request routing functionality.
    * *Web Server Gateway Interface* (WSGI) - standard specification (PEP 3333) upon which servers and python web applications/frameworks can communicate. Read more [here](https://peps.python.org/pep-3333/).
* [Bootstrap](https://getbootstrap.com/docs/5.3/getting-started/introduction/) - for the user-interface, files are hosted statically by SPYGAZER.
* `gevent`, `geventwebsocket` for client-side request routing throughout the front-end (Bottle) web application server.
* Client-side Javascript for communicating with the python WSGI websocket server.
* Made with ❤️

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

### > *Responsive Layout Positioning*
![image](https://github.com/user-attachments/assets/9aab556d-afb0-492c-8a42-6b2aecb12027)

![image](https://github.com/user-attachments/assets/787512cf-6b2f-4e9e-bb83-a08186c85d09)
