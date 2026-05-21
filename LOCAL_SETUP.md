# Instructions for setting up a local environment to run labs in place of GitHub Codespace

### NOTE: GitHub Codespaces - as detailed in the README.md file - are the preferred and recommended environment to run the labs in. Use this alternative only if you can't use the Codespace option for some reason. ##

<br><br>

These instructions will guide you through configuring a local environment that you can use to do the labs. 

<br><br>

**1. Install Git on your system if you don't already have it.**

The main Git site is [here](https://git-scm.com) with installers. 

<br>

![Getting Git](./images/local-4.png?raw=true "Getting Git")

<br><br>

**2. Install a version of Docker on your system if you don't already have one.**

You can go to [Docker.com](https://docker.com) to find out how to get setup. For Windows and Mac users, [Docker Desktop](https://www.docker.com/products/docker-desktop/) is a good option.

<br>

![Getting Docker Desktop](./images/local-3.png?raw=true "Getting Docker Desktop")

<br>

[This link](https://code.visualstudio.com/remote/advancedcontainers/docker-options) discusses alternative options for Docker in VS Code (including use of Podman).

<br><br>

**3. Install VS Code on your local machine.**

To do this, go to [this link](https://code.visualstudio.com/download) and follow the instructions for your operating system.

<br>

![Getting VS Code](./images/local-1.png?raw=true "Getting VS Code")

<br><br>

**4. Once you have Docker running and VS Code installed, find the Dev Containers extension and install it.**

<br>

In VS Code, you can use the shortcut command to open the *Extensions* view (usually SHIFT+CMD+X or SHIFT+CTRL+X) or find the *Activity Bar* and click on the *Extensions* icon.

Then, in the search box at the top of the *Extensions* view, enter "Dev Containers" and, once found, click *Install* to install the extension in VS Code.

<br>

![Installing Dev Containers extension](./images/local-2.png?raw=true "Installing Dev Containers extension")

<br>

Alternatively, you can install the extension from it [page on the Visual Studio Marketplace](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers).

<br><br>


**5. Click on the button below to open the code from this repository as a development container in your local VS Code instance.**  

If this doesn't work, you can do the alternative steps below.

<br>

&emsp;&emsp;&emsp;&emsp;Click here ➡️ 
<a href="https://vscode.dev/redirect?url=vscode://ms-vscode-remote.remote-containers/cloneInVolume?url=https://github.com/dreganism/aia-day1">
  <img src="https://img.shields.io/static/v1?label=Dev%20Containers&message=Open&color=blue&style=for-the-badge"
       alt="Open in Dev Containers" height="48">    
</a>     

<br>

**Alternative steps - only needed if clicking the button in step 5 didn't work.**

a. Use Git to clone this repository down to your machine with a command like the following.

```
git clone https://github.com/skillrepos/<repo-name>
```

<br><br>

b. Open up the cloned project in VS Code. 

There are multiple ways to do this: 
- You can drag and drop the project directory onto VS Code.
- You can open VS Code and open the folder from its menu.
- You can simply change into the cloned directory and run the command "code ."

```
cd <cloned repo dir>
code .
```

<br><br>

c. Once you open the folder/project in VS Code, VS Code should detect the devcontainer setup and prompt you about running it as a development container (usually in lower right corner). Click on "Reopen in Container".

<br>

![Starting in VS Code](./images/local-5.png?raw=true "Starting in VS Code")

<br>

d. If you get a popup about "Not all host requirements in devcontainer.json are met by the Docker daemon", you can just click *Continue* and it will probably still be fine.

![Host requirements](./images/local-6.png?raw=true "Host requirements")

<br><br>


**6. Allow the setup processing to run automatically. (May take several minutes for some projects).**

<br>

![Setup](./images/local-7.png?raw=true "Setup")

<br><br>

**7. When the processing is done, you are ready to run the labs in your local environment!**

<br><br>

---

## License and Use

These materials are provided as part of the **Enterprise AI Accelerator Workshop** conducted by **TechUpSkills (Brent Laster)**.

Use of this repository is permitted **only for registered workshop participants** for their own personal learning and
practice. Redistribution, republication, or reuse of any part of these materials for teaching, commercial, or derivative
purposes is not allowed without written permission.

© 2025 TechUpSkills / Brent Laster. All rights reserved.
