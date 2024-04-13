# nopCommerce-BDD-Automation-Framework


## Introduction
nopCommece (https://demo.nopcommerce.com/) is an E-Commerce page to buy electronic devices, computers, books, jewelry online.
- Design pattern used: page object model(POM)
- Methodology: behavior driven development(BDD)
- Gherkin language for various features of application like login, register, search results.


## Project Structure
The project is organized as follows:

- "features" package which contains the following feature files:
  - "login.feature" : Validates functionalities of the log in page;
  - "register.feature" : Validates functionalities of the register page;
  - "search_results.feature" : Verify that search results;


 - "pages" package which contains the following .py files:
   - "base_page" : contains methods used throughout the entire project, especially in the "steps" files;
   - "home_page" : contains methods used for the home page tests;
   - "login_page" : contains methods used for the log in page;
   - "register_page" : contains methods used for testing the register up functionality.
   - "search_results" : contains methods used for the search results;
  
   - "steps" package which contains the following .py files:
     - "login_steps" : contains the steps that each test on the log in page follows;
     - "register_page_steps" : contains the steps that each test on the register page follows;
     - "search_results_steps" : contains the steps that each test regarding the search bar.
     
- additional files:
  - "behave-report.html" : This HTML report is generated when running the tests.;
  - "behave.ini" :  Contains configuration for the HTML formatter;
  - "browser.py" : Sets up the browser for testing;
  - "environment.py" : Instantiates objects from the classes to be used throughout the project.


## Clone Project
Install Git Bash terminal, select a folder where you want to copy the project and then run in the Git Bash this command: "git clone https://github.com/IoanaFlore/nopCommerce-BDD-Automation-Framework.git"

## Installation
To install the required libraries, execute the following commands:
- `pip install selenium`
- `pip install behave`
- `pip install webdriver-manager`
- `pip install behave-html-formatter`

## Running the Project use the following command
-  "behave -f html -o behave-report.html" : for running the entire project
-  "behave -f html -o behave-report.html --tags=your_tag" : for running the desired tests 
