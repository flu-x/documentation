---
layout: default
title: Module Configuration
nav_order: 2
---

# Installing and Updating driver packages
------------------------------------------------------------------------------------------
Please follow the below steps to install and configure browserium in your systems and get started with Browserium.

## Installing Browserium
------------------------------------------------------------------------------------------
*   To install Browserium using PiP run the command:

	   `pip install browserium`

*   To install Browserium from GitHub run the command:

	   `pip install git+git://github.com/browserium/Browserium.git`

## Modules installed with browserium
------------------------------------------------------------------------------------------
*   **requests**
*   **selenium**
*   **wget**

Make sure you have **ssh** configured in GitHub. You can also use **https** as well to install the module. But preferrable would be if you have **ssh** configured in GitHub.

To install Browserium from GitHub using HTTPS run the command:

	pip install git+https://github.com/browserium/Browserium.git

*   To download chromedriver run the command

	   ```browserium download --driver=chromedriver```

*   To download geckodriver run the command

	   ```browserium download --driver=geckodriver```

*   To download operadriver run the command

	   ```browserium download --driver=operadriver```

## Updating Browser Drivers
------------------------------------------------------------------------------------------
*   To update chromedriver run the command

	   ```browserium update --driver=chromedriver```

*   To update geckodriver run the command

	   ```browserium update --driver=geckodriver```

*   To update operadriver run the command

	   ```browserium update --driver=operadriver```
