---
layout: default
title: Browser Instances
nav_order: 4
---

## Create instance for Chrome
------------------------------------------------------------------------------------------
Please follow the below guidelines to create a browser instance for Chrome using browserium
*      Create instance for the `ChromeDriverObject` class
*      Use the instance for `ChromeDriverObject` class to call the `set_chromedriver_object` method.
*      Create instance for the `Browser_controller` class to use the generic methods.

```python
	from browserium.generic_functions.chrome_object import ChromeDriverObject
	from browserium.generic_functions.browser_controller import Browser_controller
	from time import sleep

	class Test_1():
		def test_chromedriver_type1(self):
			chromedriver = ChromeDriverObject()
			controller = Browser_controller()
			driver = chromedriver.set_chromedriver_object()
			controller.get_url(driver, "https://www.google.co.in")
			controller.implicit_wait_time(driver, 4)
			current_url = controller.get_current_url(driver)
			print current_url
```
*      To run chromedriver with custom configurations, pass the configurations as a list of objects to the `set_chromedriver_object()` method. Refer to the codebase below as suggested.

```python
	from browserium.generic_functions.chrome_object import ChromeDriverObject
	from browserium.generic_functions.browser_controller import Browser_controller
	class Test_1():
		def test_chromedriver_type1(self):
			chromedriver = ChromeDriverObject()
			controller = Browser_controller()
			driver = chromedriver.set_chromedriver_object(chromeArgs=['--headless','--no-sandbox'])
			controller.get_url(driver, "https://www.google.co.in")
			controller.implicit_wait_time(driver, 4)
			current_url = controller.get_current_url(driver)
			print current_url
```

## Create instance for Firefox
------------------------------------------------------------------------------------------
Please follow the below guidelines to create a browser instance for Firefox using browserium
*   Create instance for the `GeckoDriverObject` class
*   Use the instance for `GeckoDriverObject` class to call the `set_geckodriver_object` method.
*   Create instance for the `Browser_controller` class to use the generic methods.

```python
	from browserium.generic_functions.gecko_object import GeckoDriverObject
	from browserium.generic_functions.browser_controller import Browser_controller
	class Test1():
		def test_geckodriver_type1(self):
			geckodriver = GeckoDriverObject()
			controller = Browser_controller()
			driver = geckodriver.set_geckodriver_object()
			controller.implicit_wait_time(driver, 4)
			controller.get_url(driver, "https://www.google.co.in")
			current_url = controller.get_current_url(driver)
			print current_url
			print driver.title
```

*       To run geckodriver with custom configurations, pass the configurations as a list of objects to the `set_geckodriver_object()` method. Refer to the codebase below as suggested.

```python
	from browserium.generic_functions.gecko_object import GeckoDriverObject
	from browserium.generic_functions.browser_controller import Browser_controller
	class Test1():
		def test_geckodriver_type1(self):
			geckodriver = GeckoDriverObject()
			controller = Browser_controller()
			driver = geckodriver.set_geckodriver_object(geckoArgs=['--headless','--no-sandbox'])
			controller.implicit_wait_time(driver, 4)
			controller.get_url(driver, "https://www.google.co.in")
			current_url = controller.get_current_url(driver)
			print current_url
			print driver.title
```

## Create instance for Opera
------------------------------------------------------------------------------------------
Please follow the below guidelines to create a browser instance for Opera using browserium
*   Create instance for the `OperaDriverObject` class
*   Use the instance for `OperaDriverObject` class to call the `set_operadriver_object` method
*   Create instance for the `Browser_controller` class to use the generic methods.

```python
	from browserium.generic_functions.opera_object import OperaDriverObject
	from browserium.generic_functions.browser_controller import Browser_controller
	class Test1():
		def test_operadriver_type1(self):
			operadriver = OperaDriverObject()
			controller = Browser_controller()
			driver = operadriver.set_operadriver_object()
			controller.implicit_wait_time(driver, 4)
			controller.get_url(driver, "https://www.google.co.in")
			current_url = controller.get_current_url(driver)
			print current_url
			print driver.title
```

## Create instance for Safari
------------------------------------------------------------------------------------------
Please follow the below guidelines to create a browser instance for Safari using browserium
*   Create instance for the `SafariDriverObject` class
*   Use the instance for `SafariDriverObject` class to call the `set_safaridriver_object` method
*   Create instance for the `Browser_controller` class to use the generic methods.

```python
	from browserium.generic_functions.safari_object import SafariDriverObject
	from browserium.generic_functions.browser_controller import Browser_controller
	class Test_1():
		def test_safaridriver_type1(self):
			safaridriver = SafariDriverObject()
			controller = Browser_controller()
			driver = safaridriver.set_safaridriver_object()
			controller.get_url(driver, "https://www.google.co.in")
			controller.implicit_wait_time(driver, 4)
			current_url = controller.get_current_url(driver)
			print current_url
			print driver.title
			driver.quit()
```
P.S: Safaridriver comes shipped with the Safari browser by default. You have to enable the `Allow Remote Automation` option from the `Develop` menu. Please check this screenshot.
![Safari](https://farm2.staticflickr.com/1738/28757957868_38fff165d4.jpg)

Keep in mind that your safari version has to be more than 10. If it is not 10 or more than 10 then please update your Safari version.

## Deleting all browser driver
------------------------------------------------------------------------------------------
To delete all browser drivers from `/usr/local/bin` run the command:

   ```python
   browserium delete --driver=all
   ```