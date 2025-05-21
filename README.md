# SPYGAZER

[![PlatinumVoyager - SpyGazer](https://img.shields.io/static/v1?label=PlatinumVoyager&message=SpyGazer&color=blue&logo=github)](https://github.com/PlatinumVoyager/SpyGazer "Go to GitHub repo")
[![stars - SpyGazer](https://img.shields.io/github/stars/PlatinumVoyager/SpyGazer?style=social)](https://github.com/PlatinumVoyager/SpyGazer)
[![forks - SpyGazer](https://img.shields.io/github/forks/PlatinumVoyager/SpyGazer?style=social)](https://github.com/PlatinumVoyager/SpyGazer)
[![License](https://img.shields.io/badge/License-The_Unlicense-blue)](https://github.com/PlatinumVoyager/SpyGazer/blob/main/LICENSE)

> [!NOTE]
> This project is undergoing active development. There is no official release date as of now. Stand by.

## 🔍 What is SPYGAZER?

SPYGAZER (PeekingGlass Server) is an HTTP-based application-layer (L7) server that provides **deep situational awareness** of the local subnetwork it operates within. It is engineered to offer a unified, interactive dashboard for observing, managing, and extending visibility into devices, protocols, and communication behaviors across a network.

Rather than passively monitor, SPYGAZER is designed to function as a **central intelligence node** — a "spyglass" into the digital terrain of the current environment.

## ✨ Key Capabilities

* **Modular Dashboard** – Dynamically view network topology, system processes, engagement tools, and backend access points.
* **Process Intelligence** – Interact with and manage server-side processes through a robust internal manager.
* **Web Shell Access** – Seamless backend shell access from within the dashboard (e.g. subshell panel, redirectable viewport).
* **Future Scope:**
  * Network Manager (Wireless AP/Client view, rogue access point handling)
  * Device Behavior Fingerprinting.
  * Live packet-based notifications or triggers.
  * Extendable modules for engagement or research actions.

### ⚙️ Architecture:
* [Bottle](https://bottlepy.org/docs/dev/) - a lightweight WSGI micro web-framework used by the web application for path/request routing functionality.
    * *Web Server Gateway Interface* (WSGI) - standard specification (PEP 3333) upon which servers and python web applications/frameworks can communicate. Read more [here](https://peps.python.org/pep-3333/).
* [Bootstrap](https://getbootstrap.com/docs/5.3/getting-started/introduction/) - for the user-interface, files are hosted statically by SPYGAZER.
* `gevent`, `geventwebsocket` - for server-side request routing throughout the front-end (Bottle) web application server.
* Client-side Javascript for communicating with the python WSGI websocket server.
* Designed for deployment on **personal, lab, or red team subnets**.
* Embedded HTTP server logic with a dynamic frontend.
* Lightweight footprint and highly customizable modules.

## 📜 Ethical Use Policy

SPYGAZER is intended **strictly for use in authorized environments** — networks you own or are explicitly permitted to audit, test, or research. While its capabilities are powerful, its purpose is to enable **defensive research, diagnostics, education, and controlled experimentation.**

Any unauthorized deployment or use may violate local, state, or federal law.

> "Power without ethics corrupts absolutely. SPYGAZER's vision is only as righteous as the hands it serves."

## 🔮 Development Philosophy

SPYGAZER is being built as both a **creative lab project** and a **potential platform for advanced security research.**
* **Public Path**: Secure, ethical, and open-source components intended for community collaboration, learning, and experimentation.
* **Private Path** *(Optional)*: Reserved features for controlled environments, adversarial emulation, and highly customized infrastructure operations.

## 📁 Repository Status
* 🛠️ Active Development.
* :closed_lock_with_key: Code is currently private.

## 📌 Author

Created and maintained by [PlatinumVoyager](https://github.com/PlatinumVoyager).

### <ins>Release?</ins> 
*To be determined.*

## 📑 Documentation
The associated documentation will be available/produced as:
   * A `.pdf` (Portable Document File) file subsequently made accessible when the project is open sourced with a public release coming in version 1.0.0.
   * A Github markdown based "wiki" page. (*NOTE*: This will be posted shortly after the `.pdf` file is integrated into this public repository)
     
   * Each subsequent main route (i.e, /spygazer/subshell, /spygazer/dashboard) will have available help upon clicking the associated button.
      * This will include general documentation for the current page, and a listing breakdown of the functionality of said page.
      * Documentation for the entire SPYGAZER web application may be built into the server directory itself at a later point in time.
<br>

## :eye: Graphical User Interface Preview
> [!WARNING]
> *All images depicted are a work-in progress and are not final.*

### <ins>Weekly Snapshot Update</ins>:
*A WSU is simply a screenshot of the current development process.*
* This snapshot instance (as seen below) has been tested and confirmed to run on a base [Raspberry PI 4](https://www.raspberrypi.com/products/raspberry-pi-4-model-b/specifications/).

<img src="https://github.com/user-attachments/assets/43fd1a56-e9ea-4777-96d5-7d0e8c723baa" width="70%" height="70%">

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
  
<img src="https://github.com/user-attachments/assets/c1315597-8f45-44cb-b945-91ffe0be6c26" width="75%" height="75%">

### > <ins>*Main Dashboard: Systemic Logger*</ins> (work-in progress)
* Customized logging utilities.
* Server-wide event specific monitoring.
  
<img src="https://github.com/user-attachments/assets/48df861b-9713-4376-b18a-3330ce26faf4" width="75%" height="75%">

### > <ins>*Process Manager*</ins> (OLD UI Mockup)
*The old user interface for the SPYGAZER Process Manager before it was programatically implemented within the primary application interface.*

It simply means this was built within a separate HTML document then ported over through the Python/JS backend. Take a look below nonetheless:
  
<img src="https://github.com/user-attachments/assets/916ed5ac-c2cb-47d0-b117-9ee91b8bd707" width="75%" height="75%">

### > <ins>*Process Manager*</ins> (Dashboard Integration OLD)
*The old UI Mockup has been successfully integrated within the primary application. This rough draft shows the evolution of complex software. Let this be known as Stage 1 of the official web interface.*

<img src="https://github.com/user-attachments/assets/d261348e-bc14-46cc-ae02-ded6d60dcc7b" width="75%" height="75%">

### > <ins>*Process Manager*</ins> (Dashboard Integration NEW)
*This sets the stage for Stage 2 of the official SPYGAZER web application interface. This is the version you will see going forward with the development cycle.*

<img src="https://github.com/user-attachments/assets/10d09a3e-f18c-4148-9f6b-005027350fc0" width="75%" height="75%">
<img src="https://github.com/user-attachments/assets/fb3938fa-3482-4a21-8138-4fbcfb8d4c60" width="75%" height="75%">
<img src="https://github.com/user-attachments/assets/6528c9ea-49e3-41ef-8086-b233e1eca3dd" width="75%" height="75%">
<img src="https://github.com/user-attachments/assets/1ddef8b2-05a4-41db-b0e2-e426609fa76d" width="75%" height="75%">
<img src="https://github.com/user-attachments/assets/c4966bc7-4e92-44ec-9bfb-e6dffed55902" width="75%" height="75%">

* Added the ability to search through processes for information which concerns the following:
   * Name of the process.
   * Status of the process: *Running*, *Sleeping*, *Idle*. (ALL supported process state types can be seen in the image below)
      * ![image](https://github.com/user-attachments/assets/a0f96036-e237-4401-bdd5-a6526f37cbc5)
   * Process states can be filtered with the click of a button via the "Process Stats" dropdown menu within the Process Managers sub-window context.
   * ANY/* other text that is contained within the bounds of the process container.
         
<hr>

### > <ins>*Websocket System Subshell*</ins> (work-in progress)
* Support for CSS (*Cascading Style Sheets*) font-family and font-size custom user defined declarations via JavaScript DOM manipulation will come before release.
  
![image](https://github.com/user-attachments/assets/3011dc6e-1d3b-4737-a063-6586e38259ee)

### > <ins>*Responsive Layout Positioning*</ins> (Mobile Operators)
> [!NOTE]
> For remote clients using a mobile device, custom JavaScript and CSS styling has been built into the application beyond that of the original bootstrap base functionality. This will correctly position elements justly to accomodate for a narrower virtual viewport.

![image](https://github.com/user-attachments/assets/9637b932-6d88-4fb9-90e7-cb0c86c3b693)

![image](https://github.com/user-attachments/assets/f9de5143-2528-4f95-afe1-92ed09f9ba44)
* `psutli_test.py` - Totally not a typo ;)

<h3><ins>Websocket Subshell Features</ins></h3>

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
