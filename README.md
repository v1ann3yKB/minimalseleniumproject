# 1. Abstract
This project (downloadable from git) is a very minimalistic Maven project to run a Selenium Java Test Case performing a simple login against the demo eCommerce website on:
https://www.saucedemo.com/

The projects simply imports via Maven Selenium, Chrome Driver and TestNG, and it consists of a signle test case LoginBasicTest.java that executes a login using the WebDriver API and verify the expected result via TestNG assertion.
The project is by purpose very simple to show a very basic setup to run Selenium automation, the pom.xml is the required Maven file with the dependencies, and the testng.xml file is the file used by TestNG to configure the test cases.


# 2. Prerequirements
- Java 1.8.x
- Maven (configured properly with Java)
- Internet connection
- Google Chrome browser
- Selenium Chrome Driver (download here: `http://chromedriver.chromium.org/downloads` and unzip and store somewhere safe the executable)
- *IMPORTANT:* please provide the selenium chrome driver full path as value of the `CHROME_DRIVER_FULL_PATH` variable inside the test case file `/src/test/java/tests/LoginBasicTest.java`, before executing the tests (see the current property value for an example).

# 3. Installation
- Checkout/download the project from the git repository into a root folder

# 4. To run the test cases
- Open a Command Line
- Go where this project was checked out (root folder)
- Run 
```
"mvn clean verify"
```
The command will clean any existing target folder, compile and build the project and run the test case.
The screen command line output will provide the test logs and information.

