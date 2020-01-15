# Assignement - Testing the Instar informatika website

For purpose of this project, I have selected a example of testing a webiste. This website is an official webshop of Instar informatika company and url is https://www.instar-informatika.hr/.

In this repository you can find few tests for trying out and testing navigation through website. Also, there are some basic functionalities like login.

Tests are written in Kotlin programming language using IntelliJ IDEA.

The test cases are following:
* Check if the header is displayed. This is the simplest test and it shows if the website is loaded correctly.
* Search for an item with search box. Probably most useful thing in every application is search engine. It easy filters all items which are interested to the user. Test works in the way that input is sent in search box and then search button is clicked. After that, results are shown in list.
* Filter items by category. If user wants see all items within some category, he can easily put mark on checkbox which represent category. In test, some categories are marked and their categories are displayed.
* Add item into cart. When user wants to buy something, he first must add it into cart and then he continues with payment. In test, random item is selected and added into cart. For the test to be successful, cart size must not be empty.
* Change tab in profile menu. This test uses login because this functionality is only available for registered users. Important thing is that user must first enter user credentials in test file to run this test. Test opens login part of website. After login, random tab in profile menu is opened. When selecting another tab, url does not change. 

To use this project, clone this repository on your computer and open it with Intellij IDEA. 

For this project you should also have ChromeDriver and FirefoxDriver (geckodriver). If you do not have them, you can download them by opening following links.

ChromeDriver: https://chromedriver.chromium.org/downloads

FirefoxDriver: https://github.com/mozilla/geckodriver/releases

When project is built successfully, to run tests you simply right click on WebTest.kt file in src/java/test package. After that click on Run ‘WebTest’ option to execute test. Once tests are finished, results will be displayed at the bottom.

Another way to run tests is to run them with command prompt. Navigate to your project directory and run ‘mvn test’ command. With this way, report file will be created which include all details of run tests. File is located in target/surefire-reports/index.html in project directory.

If there are failed tests, that means that there are bugs in application and developers should fix it in newer versions.


