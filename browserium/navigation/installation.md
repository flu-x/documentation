---
layout: default
title: Module Configuration
nav_order: 2
---

# Installing and Updating driver packages
------------------------------------------------------------------------------------------
Please follow the below steps to install and configure flexibox in your systems and get started with Flexibox.

## Installing Flexibox
------------------------------------------------------------------------------------------
*   To install Flexibox using PiP run the command:

	   `pip install flexibox`

*   To install Flexibox from GitHub run the command:

	   `pip install git+git://github.com/flexibox/Flexibox.git`

## Modules installed with Flexibox
------------------------------------------------------------------------------------------
*   **requests**
*   **selenium**
*   **wget**

Make sure you have **ssh** configured in GitHub. You can also use **https** as well to install the module. But preferrable would be if you have **ssh** configured in GitHub.

To install Flexibox from GitHub using HTTPS run the command:

	pip install https://github.com/flu-x/flexibox.git

*   To download chromedriver run the command

	   ```flexibox download --driver=chromedriver```

*   To download geckodriver run the command

	   ```flexibox download --driver=geckodriver```

*   To download operadriver run the command

	   ```flexibox download --driver=operadriver```

## Updating Browser Drivers
------------------------------------------------------------------------------------------
*   To update chromedriver run the command

	   ```flexibox update --driver=chromedriver```

*   To update geckodriver run the command

	   ```flexibox update --driver=geckodriver```

*   To update operadriver run the command

	   ```flexibox update --driver=operadriver```
