<h1 align="center">  Automation </h1>
<h1 align="center">**Robot Framework for Mobile UI Automation** </h1>

  ***Introduction:-***
   - Robot Framework is a test automation framework that makes it easy for QA teams to manage acceptance testing and acceptance test-driven development (ATDD).
   - It has simple plain text syntax and it can be extended easily with libraries implemented using Python or Java.
  
   - See ```https://robotframework.org/``` for Robot Framework home page

**Who is this repository for?**
 - This repository is for newbies to Robot Framework interested in automating the mobile UI.
##  🛠️ Installation

**👉Install python with PIP:-**
 - Visit the below website to download Python for your operating system.
                       ```https://www.python.org/downloads/```
 - You can click on ‘Install Now' to install the default package. It comes with pip, IDLE, and documentation.
 - Select option ‘Add Python <version> to PATH'that will automatically update the path of Python in environment variables.
 - After installation check if Python and pip are correctly installed open the command prompt, and run the below command.
```
    python --version
``` 
``` 
    pip --version 
```
    
 - If in condition the path is not set then go to enviornment variables then click on PATH in user & system variable both & add
                    ```D:\Python\``` , ``` D:\Python\Scripts\``` , ``` D:\Python\Lib\site-packages\robot```, ```D:\Python\Tools ```
                    & save it.

**👉Install Java jdk**
 - Search java jdk,
                LINK TO DOWNLOAD: https://www.oracle.com/java/technologies/javase/javase-jdk8-downloads.html
 - Install it & add to environment Variable, 
   - Add new System variable with name JAVA\_HOME & 
                 Paste                  
                 ```
                 C:\Program Files\Java\jdk1.8.0\_27 
                 ``` ,
                 & 
                 ```
                 C:\Program Files\Java\jdk1.8.0\_271\bin
                 ``` .
 - After installation check if java is correctly installed open the command prompt, and run the below command.
```
    java -version
```

**👉Install node js**
 - Search node js,
 - Click on PATH in system variable & add
   - ```C:\Program Files\nodejs```
   - ```C:\Program Files\nodejs\node\_modules```
   - ```C:\Program Files\nodejs\node\_modules\npm```
 - After installation check if node js is correctly installed open the command prompt, and run the below command.
		        ```node -v```

**👉Install appium:-**
 - In cmd type 
``` 
npm  install -g appium
```
    
 - After installation check if appium is correctly installed open the command prompt, and run the below command.
```
    appium --version
```
    
 - To check whether installation is done proper or not open the command prompt, and run the below command.
```
    npm -g appium doctor
```
            
**👉Install appium libraries:-**
 - Install appium library for automation
 - Type in cmd 
```
    pip install robotframework appium library
```

**👉Install appium standalone application:**
 - Download standalone application appium
		LINK TO DOWNLOAD:```https://github.com/appium/appium-desktop/releases/tag/v1.20.2```, 
           OR DOWNLOAD THE LATEST ONE ```https://github.com/appium/appium-desktop/releases/latest```

**👉Install Android studio:-**
 - You can Install full package if want to create emulator to run application
                LINK TO DOWNLOAD: ```https://developer.android.com/studio```
 - After installation add environment variable to path--->
    - create new in user variable  & name it ANDROID\_HOME
    - copy path ```C:\Users\username\AppData\Local\Android\Sdk``` & paste it.
 - Go to PATH in system variable  & add these paths in it:
    - ```C:\Users\username\AppData\Local\Android\Sdk\platforms```
    - ```C:\Users\username\AppData\Local\Android\Sdk\platform-tools```
    - ```C:\Program Files\Android\Android Studio\bin```
    - ```C:\Users\username\AppData\Local\Android\Sdk\tools\bin```
    - ```C:\Users\username\AppData\Local\Android\Sdk\emulator```
    - ```C:\Users\username\AppData\Local\Android\Sdk\build-tools  to execute commands inside this folder```


**👉Installation of IDE**
 * Pycharm with intellibot plugin
    - Navigate to ```https://www.jetbrains.com/pycharm/download/``` and download it.
    - Click next to install and select checkbox for Create 64-bit shortcut on Desktop.
    - Go to File>>Settings>>Plugins and  search for intellibot and install IntelliBot, Robot Framework Support plugin.
 * Eclipse download
    - Navigate to ```https://www.eclipse.org/downloads/``` and download Eclipse Integration with RobotFramework and RED
    - Open Eclipse, Goto Help >> Eclipse Marketplace
    - Search for RED, you will get RED Editor for RobotFramework, Install this and restart the eclipse

 * Installing PyDev for Eclipse
    - In Eclipse, click Help > Eclipse Marketplace.
    - Search for "PyDev" and click install and then restart eclipse when prompted.



**👉Libraries Installation**
 - Open Command Prompt (cmd) and run the below command.
```
    pip install robotframework
```

**Make sure all the packages inside the project interpreter are installed**
 - To verify follow the path
                    File>Settings>Project interpreter
    - ![image](https://user-images.githubusercontent.com/87467505/156704202-eb554be0-ab4f-48de-938b-6f266bbd1e2f.png)

## 1. What exactly in it?
 * Introduces the basic Robot Framework syntax, how tests are executed, and how logs and reports look like
 * Framework Architecture:
    We have two below libraries:-
     - 1. Robot Standard Libraries: These test libraries are distributed with Robot Framework
     - 2. Robot Referenced Libraries : These are external Libraries installed by pip.
 * Folders
   - a) External keywords : This section is used to set up the common functions which will be used throughout the framework like locators,swipe  etc.
   - b) Resources: This section is used to set up all the global level parameters which will be used throughout the framework like libraray etc.
   - c) Test cases: This section is where all the tests are automated.
     * Package is created with name RegressionSuite and all the tests are automated in it.
     * For Ex: Under Test cases directory we have sub directory called RegressionSuite.
     * and under RegressionSuite we have tests Mobile UI with the following tests are mentioned below
    ![image](https://user-images.githubusercontent.com/87467505/156704646-376e46d6-b993-43ed-8266-22eb0f2f45b1.png)
  - d) TestData: This section will contain stored test data in form of json or excel which will be used by our test.
  - f) Json files: This section contains json file which contains all locators in the form of keyvalue pair.
    * For Ex. Elements.json
  - g) Report: This section contains report.html and log.html file stored in it.
  - h) Snapshots: This section contains all the screenshots which are taken on testcases pass and fail condition.
    
## <img src="https://media.giphy.com/media/iY8CRBdQXODJSCERIr/giphy.gif" width="30px"> Usage
    
 - When using Robot Framework, it is generally recommended to write as easy-to-understand tests as possible.
 - This is illustrated by the following sample example
 - _Setting section_ contains all the required libraries that are required by the test
```
*** Settings ***
Library        AppiumLibrary
Resource       ../../Resources/Library.robot
```
 - Variables are used to hold a value, which can be used in test cases
```
*** Variables ***
${URL}  http://172.16.52.125:4723/wd/hub
```
    
```
*** Test Cases ***
[Documentation]  Test Cases for Login module
TC\_001- Application start and close						//Testcase name
[Tags]  Regression								//User defined tagging for the particular testcase.
Given user\_open\_application    						//User defined global keyword maintained in library.robot file
${username\_text} =    Read\_Element\_Locator  Login.username\_textbox\_xpath		//User defined keyword to fetch the keyvalue through the jsonpath
${paswword\_text} =    Read\_Element\_Locator  Login.password\_textbox\_xpath		//User defined keyword to fetch the keyvalue through the jsonpath
${send\_button} =      Read\_Element\_Locator  Login.login\_button\_id			//User defined keyword to fetch the keyvalue through the jsonpath
${account\_section} =  Read\_Element\_Locator  Login.account\_button\_xpath		//User defined keyword to fetch the keyvalue through the jsonpath
${logout} =           Read\_Element\_Locator  Login.logout\_xpath			//User defined keyword to fetch the keyvalue through the jsonpath
${rows}=              Read\_Number\_Of\_Rows  validlogin				//User defined keyword to fetch the value from the particular row through the excel sheet
FOR  ${i}  IN RANGE  1  ${rows}+1						//Using loop to iterate the value through the different rows
${username}=  Read\_Excel\_Data\_Of\_Cell  validlogin  ${i}  1			//User defined keyword to fetch the value from the particular row through the excel sheet
${password}=  Read\_Excel\_Data\_Of\_Cell  validlogin  ${i}  2			//User defined keyword to fetch the value from the particular row through the excel sheet
When Input Text  xpath=${username\_text}  ${username}				//Feeding the data in the username input field through the excel sheet
When Input Text  xpath=${paswword\_text}  ${password}				//Feeding the data in the password input field through the excel sheet
When click element  id=${send\_button}					//Clicking on the send button
when wait until page contains element  xpath=${account\_section}  20		//Using waits
When capture page screenshot  D:/pycharm/PyCharm Community Edition 2019.3.4/robotautomation/snapshot/TC\_001.png 		//Capturing the screenshot
When Click Element  xpath=${account\_section}				//Click on the account section
When Click Element  xpath=${logout}					//Clicking on the logout button
Then user\_close\_application							//User defined global keyword maintained in library.robot file
```



- Running tests:
 - Tests are executed from the command line using the robot command
```
    robot <Foldername>/<TestName>.robot
```
For Ex: 
```
    robot TC_001- Application start and close.robot
```
- Generated results:
 - After running tests you will get report and log in HTML format.
   - 1. ```report.html```
   - 2. ```log.html```










