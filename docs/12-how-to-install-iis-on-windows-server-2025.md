---
Category: 1
---
# How to install IIS on Windows Server 2025

In "Server Manager" (under "Dashboard"), click "Add roles and features":

![](img/12/1.png)

In the "Add Roles and Features Wizard" dialog, "Before you Begin" section, click the "Next" button:

![](img/12/2.png)

In the "Installation Type" section, select "Role-based or feature-based installation":

![](img/12/3.png)

In the "Server Selection" section, select "Select a server from the server pool", select your server, and click the "Next" button:

![](img/12/4.png)

In the "Server Roles" section, select "Web Server (IIS)":

![](img/12/5.png)

In the dialog "Add features that are required for Web Server (IIS)", click the "Add features" button:

![](img/12/6.png)

Back in the "Server Roles" section, click the "Next" button:

![](img/12/7.png)

In the "Features" section, click the "Next" button:

![](img/12/8.png)

In the "Web Server Role (IIS)" section, click the "Next" button:

![](img/12/9.png)

> [!NOTE] The following (enabling the "Application Initialization" feature) is needed for the "Enable preload" web-site setting to work (see instructions for installing OwnCDN) - which ensures that OwnCDN startup as soon as the application pool / website starts.

In the "Web Server Role (IIS) / Role Services" section, scroll down and expand "Application Development", and check "Application Initialization", and click the "Next" button.


![](img/12/10.png)

In the "Confirmation" section, click the "Install" button:

![](img/12/11.png)

And finally, after the installation completes, click the "Close" button:

![](img/12/12.png)

