# Selenium-Playground-Table-Search-Demo

README for Selenium Automation Script
Overview
This script is created to automate testing a web application using Selenium with Python. It includes the setup for ChromeDriver and a test case to validate search functionality on a website.
________________________________________
Steps Followed
1.	Setup
o	First, I installed Selenium using pip: 
o	pip install selenium
o	Then, I downloaded the ChromeDriver that matches the version of the Chrome browser installed on my system. To find the correct version, I checked the browser version at chrome://settings/help and downloaded the driver from here.
2.	Configuring the Path
o	I provided the exact path to chromedriver.exe in the script. Here’s how I set it up: 
o	service = Service(executable_path=r"C:\\Users\\windows\\PycharmProjects\\Selenium Project\\chromedriver.exe")
o	driver = webdriver.Chrome(service=service)
3.	Testing
o	I wrote a test case using pytest to ensure the search functionality of the web application works as expected.
o	To run the script, I navigated to the directory and used the command: 
o	pytest qa_selenium_test.py
________________________________________
Best Practices Followed
•	Version Matching: Ensured that the ChromeDriver version matches the Chrome browser version to avoid compatibility issues.
•	Explicit Driver Path: Used an explicit path to the ChromeDriver executable for consistency and ease of troubleshooting.
•	Reusable Setup: Kept the configuration separate from test logic for better maintainability and readability.
•	Error Handling: Addressed driver setup errors, such as NoSuchDriverException, by ensuring the driver was executable and properly set up.
________________________________________
How to Run the Script
1.	Make sure Python, Google Chrome, and ChromeDriver are installed.
2.	Update the script with the correct path to your chromedriver.exe file.
3.	Navigate to the project directory where your script is located.
4.	Run the script using this command: 
5.	pytest qa_selenium_test.py 
________________________________________
Validation
Once the script runs, the Chrome browser should open automatically, and the test case should execute successfully. If there are issues, the error messages in the terminal will help in troubleshooting.

