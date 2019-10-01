# JPMC UI Automation Test
## Please go through the below to understand the framework and how to setup and run the test.
### Feature/Test 
````
As a user, I want to validate news article from guardian news website on similar resources, 
so that I can confirm that the news article is not FAKE news
````

````
Framework setup
````
````
* Selenium webDriver
* Java - programming language
* Chrome webdriver browser
* POM
* Cucumber
* Java 1.8
* Maven - build management tool
* IDE - IntelliJ IDEA
````
### To run the test:
````
1. Download, install and setup Java SDK (Java 1.8) on your PC.
2. Ensure that you have the latest version of chrome browser on your local computer
3. Install IntelliJ IDEA on you PC, go to File - Project Structure - Project, 
   then point it to the Java 8 SDK, click apply & ok button.
4. On your drive, crate a folder and give it a name i.e 'MuyiTest' 
5. Go to Terminal/cmd, change directory into the folder created.
6. Use git comman "git clone https://github.com/Muyiadesote/jpmc_UITest.git" to Clone the test 
   framework into the created folder on your PC.
7. Launch IntelliJ, go to File - select Open and point to the cloned test framework, then select 
   the pom.xml file (MAC)- This will load up the project.
8. Go to File on IntelliJ, Project Structure, select Project - (Project SDK) and point to your 
   java 1.8 location - Apply and click on OK.
9. Go to Build at the top of IntelliJ and select Build Project.
10. Once the has built successfully, go to 'src\test\java\com\Jpmc\TestRunner' 
    right click on it and select "Run 'TestRunner' - this will start to execute the test.
11. You may also wish to run the test from Terminal with 'mvn test' command - provided you 
   have maven installed and correctly setup on your pc within the environment variables.
````
````
Please note: If the test fails (Chromedriver is not executable) - please download 
Google chromedriver for mac, version 77.0 from https://www.seleniumhq.org/download/
Add it to the Drivers package src/Drivers. 
Then go to src\main\java\com\Jpmc\DriverInstance.java, line 27 and update the driver
name accordingly.
Repeat step 9 & 10 from above.
````
