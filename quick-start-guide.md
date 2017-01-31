## Try WebPivotTable live demo applications

We have some live demo applications for you to try all functionalities of WebPivotTable. They are for demo purpose only, we don't save any data on our server and we don't provide commercial support for the usage of them. We suggest you load insensitive source data only or just use sample data within these applications.

Please go to [Demo Page](http://webpivottable.com/demo/) to open these applications. There are lots of animation demos on this page either. If you don't know how to use WebPivotTable, watch those animation demos first.

## Install your own WebPivotTable application

If you had been convinced by live demo applications and would like to install a similar web application for internal use, please go to [Download Page](http://webpivottable.com/download/) to download a WebPivotTable free edition and follow list below steps to install it on your computer or your server.

_To install WebPivotTable free edition, you don't need to have a server machine. You can install it on your computer and use it just by yourself or by others who can connect to your computer. Of course, if you are in a cooperation network, either it is a local area network or an Intranet network, it would be better to install WebPivotTable on a server machine so that anybody within this network can use it all the time without interruption.
_
_WebPivotTable free edition is totally free to be used by any person or any company, either for personal use or for commercial use.
_
WebPivotTable free edition depends on [NodeJS](https://nodejs.org/) to start an internal web server. You need have NodeJS installed on the computer or the server which you will install WebPivotTable on. Please go to [Install NodeJS](https://nodejs.org/en/download/) to download a proper NodeJS installer then run the installer following the instruction on the screen.

_To check whether NodeJS had been installed successfully or not, [open a Command Prompt console](http://windows.microsoft.com/en-ca/windows-vista/open-a-command-prompt-window)(Windows system) or a terminal (linux/unix/Mac osx) and input command "node -v". If NodeJS had been installed, a correct NodeJS version will show on the console/terminal._

If NodeJS had been installed successfully, you can continue to install WebPivotTable free edition now:

### On Windows

Run your downloaded WebPivotTable free edition windows installer, follow the instruction on the screen.

There will be two shortcut icons on the desktop of Windows, one will start the back end web server, another will open WebPivotTable application in your default internet browser. Click the first one and keep opened console running, then click another shortcut icon. If you see WebPivotTable page opened in your browser, the installation is done successfully.

_You can input "http://localhost:8002" into the address bar of any internet browser to open WebPivotTable as well._

### On Linux/Unix/Mac OSX

Unzip your downloaded WebPivotTable package under any directory, for example, unzip the whole package under "~/WebPivotTable" directory.

Open a terminal, switch to that directory:




```
~>cd ~/WebPivotTable

```


Run "npm install" to install necessary NodeJS modules:




```
~/WebPivotTable>npm install

```


Then, start the back end web server:




```
~/WebPivotTable>node app

```


Keep this terminal opening, open any internet browser, input "http://localhost:8002" into the address bar. If you see WebPivotTable page opened in your browser, the installation is done successfully.

To access this installed WebPivotTable application from other computers within the same network, you need know IP address of the computer or the server which you installed WebPivotTable on. [Here](http://www.howtofindmyipaddress.com/) is a good instruction on how to check IP address. At other computers, open any internet browser, input "http://[your server IP address]:8002" into the address bar. For example, if that IP address is 192.168.0.1, then the link to WebPivotTable application page will be "http://192.168.0.1:8002".

## What's Next?

Installed a free edition WebPivotTable application is enough for many users. But you may need more, for example, you have a web site or web application already, you would like to embed WebPivotTable into it, or you don't want load source data from user interface every time, you would like to be able to load them from server or even from your Database system. All these requirements are addressed by WebPivotTable component edition. See [Integration Guide](/webpivottable-integration-guide.md) for more details.