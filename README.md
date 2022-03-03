# Automation
**Robot Framework for Mobile UI Automation**

## Introduction:-
    Robot Framework is a test automation framework that makes it easy for QA teams to manage acceptance testing and acceptance test-driven development (ATDD).
    It has simple plain text syntax and it can be extended easily with libraries implemented using Python or Java.
    See https://robotframework.org/ for Robot Framework home page

## Who is this repository for?
      This repository is for newbies to Robot Framework interested in automating the mobile UI.
## Installation
     a)Install python with PIP
          1. Visit the below website to download Python for your operating system
                       https://www.python.org/downloads/
          2. You can click on ‘Install Now' to install the default package. It comes with pip, IDLE, and documentation.
          3. Select option ‘Add Python <version> to PATH'that will automatically update the path of Python in environment variables.
          4. After installation check if Python and pip are correctly installed open the command prompt, and run the below command.
                ```
                python --version
                pip --version
                ```
          5. If in condition the path is not set then go to enviornment variables then click on PATH in user & system variable both & add
                    ```
                    D:\Python\
                    D:\Python\Scripts\
                    D:\Python\Lib\site-packages\robot
                    D:\Python\Tools 
                    ```
                    & save it.

   b)Install Java jdk
        1. Search java jdk
              LINK TO DOWNLOAD: https://www.oracle.com/java/technologies/javase/javase-jdk8-downloads.html
        2. Install it & add to environment Variable
              Add new System variable with name JAVA\_HOME & 
              Paste 
              ```
              C:\Program Files\Java\jdk1.8.0\_27 
              ```
              & 
              ```
              C:\Program Files\Java\jdk1.8.0\_271\bin
              ```
`		`3. After installation check if java is correctly installed open the command prompt, and run the below command.

`		`java -version

`	`c) Install node js



`		`1.Search node js\

`		`LINK TO DOWNLOAD:https://nodejs.org/en/download/

`		`2.Install it and set the evironment variables.

`		 `Click on PATH in system variable & add

`		 `C:\Program Files\nodejs

`		 `C:\Program Files\nodejs\node\_modules

`		 `C:\Program Files\nodejs\node\_modules\npm



`		`3.After installation check if node js is correctly installed open the command prompt, and run the below command.

`		`node -v

`	`d) Install appium

`		`1.In cmd type npm  install -g appium

`		`2.After installation check if appium is correctly installed open the command prompt, and run the below command.

`		`appium --version

`		`3.To check whether installation is done proper or not open the command prompt, and run the below command.

`		`npm -g appium doctor

`	`e) Install appium libraries

`		`1Install appium library for automation

`		`Type in cmd 'pip install robotframework appium library'

`	`f) Install appium standalone application

`		`1.Download standalone application appium

`		`LINK TO DOWNLOAD:https://github.com/appium/appium-desktop/releases/tag/v1.20.2
           OR DOWNLOAD THE LATEST ONE https://github.com/appium/appium-desktop/releases/latest

`	`g) Install Android studio

`		`1.You can Install full package if want to create emulator to run application

`		`LINK TO DOWNLOAD: https://developer.android.com/studio

`		`2.After installation add environment variable to path--->

`		`create new in user variable  & name it ANDROID\_HOME

`		`copy path C:\Users\username\AppData\Local\Android\Sdk & paste it.

`		`3.Go to PATH in system variable  & add these paths in it:

`		`C:\Users\username\AppData\Local\Android\Sdk\platforms

`		`C:\Users\username\AppData\Local\Android\Sdk\platform-tools

`		`C:\Program Files\Android\Android Studio\bin

`		`C:\Users\username\AppData\Local\Android\Sdk\tools\bin

`		`C:\Users\username\AppData\Local\Android\Sdk\emulator

`		`C:\Users\username\AppData\Local\Android\Sdk\build-tools  to execute commands inside this folder


`	   `f) Installation of IDE

`		`A) Pycharm with intellibot plugin

`	  		`1.Navigate to https://www.jetbrains.com/pycharm/download/ and download it.



`	  		`2.Click next to install and select checkbox for Create 64-bit shortcut on

`			 `Desktop.



`	   		`3. Go to File>>Settings>>Plugins and  search for intellibot and install IntelliBot, Robot Framework Support plugin





`		`B) Eclipse download

`	   		`1. Navigate to https://www.eclipse.org/downloads/ and download Eclipse

`	   		`Eclipse Integration with RobotFramework and RED

`	   		`1. Open Eclipse, Goto Help >> Eclipse Marketplace

`	   		`2. Search for RED, you will get RED Editor for RobotFramework, Install this and restart the eclipse



`	  		 `Installing PyDev for Eclipse

`	 		 `1. In Eclipse, click Help > Eclipse Marketplace.

`	   		 `2. Search for "PyDev" and click install and then restart eclipse when prompted



`	 `g) Libraries Installation

`		 `a)Open Command Prompt (cmd) and run the below commands

`	  		 `pip install robotframework

`	`h) Make sure all the packages inside the project interpreter are installed.

`		`a)To verify follow the path

`			`File>Settings>Project interpreter



`		`Appium-Python-Client	0.50	2.0.0

`		`decorator		4.4.2	5.1.0

`		`docutils			0.16	0.18

`		`et-xmlfile			1.0.1	1.1.0

`		`jdcal			1.4.1	1.4.1

`		`jsonpath			0.82	0.82

`		`kitchen			1.2.6	1.2.6

`		`openpyxl			3.0.3	3.0.9

`		`pip			19.2.3	21.3.1

`		`robotframework		3.1.2	4.1.2

`		`robotframework-appiumlib	1.5.0.4	1.6.3

`		`selenium			3.141.0	4.0.0

`		`setuptools		41.2.0	59.1.1

`		`six			1.14.0	1.16.0

`		`urllib3			1.25.8	1.26.7





1. What exactly in it?

`	`Introduces the basic Robot Framework syntax, how tests are executed, and how logs and reports look like



`	`Framework Architecture:

`	`We have two below libraries

`		`1. Robot Standard Libraries: These test libraries are distributed with Robot Framework

`		`2. Robot Referenced Libraries : These are external Libraries installed by pip.

`	`Folders

`		`a) External keywords : This section is used to set up the common functions which will be used throughout the

`		   `framework like locators,swipe  etc.

`		`b) Resources: This section is used to set up all the global level parameters which will be used throughout the

`		   `framework like libraray etc.

`		`c) Test cases: This section is where all the tests are automated

`			`Package is created with name RegressionSuite and all the tests are automated in it.

`			`For Ex: Under Test cases directory we have sub directory called RegressionSuite.

`		   	`and under RegressionSuite we have tests

`		   	`Mobile UI with the following tests are mentioned below



`		      	`Modules							Tests



`			`1. What are you Looking For?				Validating what are you looking for section.

`			`2.Notifications					Validating the notification.

`			`3.App Integration					Validating the app inegration.

`			`4.Classes						Signing up for the classes.

`			`5.Programs					Signing up for the programs.

`			`6.Pay My Bill					Paying the unpaid amount

`			`7.Check-in history					Checking the login history

`			`8.Profile Information				Checking the profile section

`			`9.Barcode(iOS)					Clicking on the barcode icon

`			`10.Your's favorite					Checking the favorite classes

`			`11.Reserve Again					Checking the classes for reserve again

`			`12.Greeting text					Validating the greeting text

`			`13.My schedule					Checking the schedule of the events

`			`14.Upcoming					Validating the events

`			`15.Credit card expired				Validating expired credit cards

`			`16.Statements					Validating the purchased statements

`			`17.Payment methods				Checking the payment methods

`			`18.Packages					Purchasing the packages

`			`19.Package changes				Purchasing the packages

`			`20.Profile Screen					Validating the profile

`			`21.Switch Profile					Switching the profile

`			`22.App feedback					Checking the app feedback

`			`23.Terms & Privacy					Checking the terms and privacy

`			`24.Login Module(Register now,try us,Forgot Password?)	Validating the login,registernow,tryus,forgot password link

`			`25.What's Happening ?				Validating the club annoucements

`			`26.Hero Image					Validating the hero image

`			`27.Login Information				Validating the login info

`			`28.Reservations 					Reserving the events

`			`29.Capacity Counter 				Validating the club capacities

`			`30.Club Locations					Checking the club locatons

`			`31.My Packages - Android & IOS			Validating the my packages

`			`32.Waitlist					Validating the waitlist feature under classes


`		`d) TestData: This section will contain stored test data in form of json or excel

`		`which will be used by our test.

`		`f) Json files: This section contains json file which contains all locators in the form of keyvalue pair

`		`For Ex. Elements.json

`		`g) Report: This section contains report.html and log.html file stored in it.

`		`h) Snapshots: This section contains all the screenshots which are taken on testcases pass and fail condition.




1. Usage

`	`When using Robot Framework, it is generally recommended to write as easy-to-understand tests as possible.

`	`This is illustrated by the following sample example

`	 `Setting section contains all the required libraries that are required by the test

`		`\*\*\* Settings \*\*\*

`		`Library        AppiumLibrary

`		`Resource       ../../Resources/Library.robot



`	`Variables are used to hold a value, which can be used in test cases

`		`\*\*\* Variables \*\*\*

`		`${URL}  http://172.16.52.125:4723/wd/hub



`	`\*\*\* Test Cases \*\*\*

`	`[Documentation]  Test Cases for Login module

`	 `TC\_001- Application start and close						//Testcase name

`	`[Tags]  Regression								//User defined tagging for the particular testcase.

`	`Given user\_open\_application    						//User defined global keyword maintained in library.robot file

`	`${username\_text} =    Read\_Element\_Locator  Login.username\_textbox\_xpath		//User defined keyword to fetch the keyvalue through the jsonpath

`	`${paswword\_text} =    Read\_Element\_Locator  Login.password\_textbox\_xpath		//User defined keyword to fetch the keyvalue through the jsonpath

`	`${send\_button} =      Read\_Element\_Locator  Login.login\_button\_id			//User defined keyword to fetch the keyvalue through the jsonpath

`	`${account\_section} =  Read\_Element\_Locator  Login.account\_button\_xpath		//User defined keyword to fetch the keyvalue through the jsonpath

`	`${logout} =           Read\_Element\_Locator  Login.logout\_xpath			//User defined keyword to fetch the keyvalue through the jsonpath

`	`${rows}=              Read\_Number\_Of\_Rows  validlogin				//User defined keyword to fetch the value from the particular row through the excel sheet

`	`FOR  ${i}  IN RANGE  1  ${rows}+1						//Using loop to iterate the value through the different rows



`	`\  ${username}=  Read\_Excel\_Data\_Of\_Cell  validlogin  ${i}  1			//User defined keyword to fetch the value from the particular row through the excel sheet

`	`\  ${password}=  Read\_Excel\_Data\_Of\_Cell  validlogin  ${i}  2			//User defined keyword to fetch the value from the particular row through the excel sheet

`	`\  When Input Text  xpath=${username\_text}  ${username}				//Feeding the data in the username input field through the excel sheet

`	`\  When Input Text  xpath=${paswword\_text}  ${password}				//Feeding the data in the password input field through the excel sheet

`	`\  When click element  id=${send\_button}					//Clicking on the send button

`	`\  when wait until page contains element  xpath=${account\_section}  20		//Using waits

`	`\  When capture page screenshot  D:/pycharm/PyCharm Community Edition 2019.3.4/robotautomation/snapshot/TC\_001.png 		//Capturing the screenshot

`	`\  When Click Element  xpath=${account\_section}				//Click on the account section

`	`\  When Click Element  xpath=${logout}					//Clicking on the logout button

`	`Then user\_close\_application							//User defined global keyword maintained in library.robot file



\8. Running tests:



`	`Tests are executed from the command line using the robot command

`	`robot <Foldername>/<TestName>.robot



`	`For Ex: robot TC\_001- Application start and close.robot



\9. Generated results

`	`After running tests you will get report and log in HTML format



`	`1.report.html

`	`2.log.html










