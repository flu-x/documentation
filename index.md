---
layout: default
title: Home
nav_order: 1
---

# Flexibox
------------------------------------------------------------------------------------------

<!-- ![Flexibox logo](https://live.staticflickr.com/65535/50236270473_9e9e3bfce5.png) -->

**Flexibox** is the a selenium wrapper for all **browsers** and **browser** **configurations**. This module is a single end point to access all the browser drivers and as well as the webdriver object for all the respective browsers along with the installation of your **selenium** module.

[Get Started](https://browserium.in/browserium/navigation/installation.html){: .btn .btn-purple }
[View it on GitHub](https://github.com/flu-x/flexibox){: .btn .btn-blue }
[View it on PyPi](https://pypi.org/project/flexibox/){: .btn .btn-green }

## Problem Statement
------------------------------------------------------------------------------------------
With the very fast pace of development, it has now become very important to have regular release cycle and with it it should be also kept in mind that we do a quality release. For this reason we have to have our tests automated as well so that we can have a centralised reports for regressions and other flaws in the system at the end of each build.

Now, for a stable build we have to check that our application is compatible with different browsers and platforms. When we start implementing a framework based out of Selenium WebDriver, for the code to get executed in different browsers we have to configure each of the browsers separately and make a call to the browser based on the requirement.

## The Idea
------------------------------------------------------------------------------------------
The problem statement that has been defined above was the reason I took out time to ease this entire process of setting up the browser drivers and the respective configurations for each browser. What if this process can be reduced down into few steps of execution? That is how I ended up with the idea and the implementation of **Flexibox**.

## Features covered up by 'Flexibox'
------------------------------------------------------------------------------------------
*   One step to **download** the required browser drivers.
*   One step to **update** the required browser drivers.
*   Create a **single** **instance** for your required browser object. No more code required to configure your browsers separately.
*   A set of browser related **generic** **functions** that can be utilised for debugging as well as for achieving the required functionalities and reduce efforts.
*   You can run browsers **Chrome** and **Firefox** using custom configurations by passing the configurations as a list of objects. The module should automatically handle all custom configurations.

## Flexibox by functionality
------------------------------------------------------------------------------------------

![functionality screenshot](https://farm2.staticflickr.com/1750/41853754714_971a727962.jpg)

There are two ways in which you can use Flexibox.

*   Download the required browser driver, create instance for the specific browser driver class.
*   Download the required browser driver, create instance for the specific browser driver class, create instance for the browser controller class and use the generic functions to get started with your framework.

You can refer to the above diagram for reference.

[![Netlify Status](https://api.netlify.com/api/v1/badges/57a23065-8f12-47d2-bbcb-c83b6988adee/deploy-status)](https://app.netlify.com/sites/flexibox/deploys)