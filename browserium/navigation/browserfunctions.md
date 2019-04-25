---
layout: default
title: Browser Functions
nav_order: 3
---

# Browser Controller class by functionality
--------------------------------------------------------------------
The `Browser Controller` class provides you with some eccentric methods that can be utilised to achieve the required functions.

* `get_url(driver, url)`: request the required url entered. Pass the required driver object and the 'url' as parameters.

* `implicit_wait_time(driver, time)`: Apply implicit wait before the dom loads. Pass the required driver object and the time as parameters.

* `set_window_size(driver, height, width)`: Set the window size for the current running browser. Pass the required driver object, height and the width of the window.

* `get_current_url(driver)`: Get the current url. Pass the required driver object as parameter.

* `get_network_requests(driver)`: Get all the network requests for the current page. Pass the required driver object as parameter.

* `performance_metrics(driver)`: Get required page performance data. Pass the required driver object as parameter.

* `check_console_logs(driver)`: Get all console logs. Pass the required driver object as parameter.

* `get_page_source(driver)`: Get the current page source. Pass the required driver object as parameter.

* `get_site_cookies(driver)`: Get all the site cookies. Pass the required driver object as parameter.

* `apply_fluent_wait(self, driver, fluent_wait_time)`: Apply conditional wait based on element locator. Pass the driver object and the fluent wait time (timeout) as an argument

* `apply_explicit_wait_time(self, sleepTime)`: Apply hard wait or explicit wait. Pass the explicit wait time as an argument.

* `get_current_url(self, driver)`: Get the current URL of the page. Pass the driver object as an argument.

* `set_window_size(self, driver, height, width)`: Set the window size of your browser. Pass the driver object, height and width as an argument.