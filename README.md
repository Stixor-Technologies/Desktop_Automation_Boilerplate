# Playwright End-to-end Test

## About

The purpose of this repo is to create a structured playground for automating end-to-end tests for the a desktop application

## Project structure

Project implements Page Object Pattern architecture as it's Playwright.

* **tests:** definition of test suites and scenarios

* **conftest.py:** allows you to define fixtures, plugins, and hooks that can be shared across multiple test files in a
  subdirectories.

* **mainscript:** Main code that calls all the fixtures and run them

* **pages:** main project library combines pages construction and behaviour in `page_objects`, pages locator
  definition and generation in `locators` and common elements like navbars or textinputs in `elements`.

* **run_tests:** A batch file that execute all test cases and create a report This consist of commands

* **csv file:** to read the data from an external file, all the data is kept in different csv files. In this case the user credentials are kept in "credentials.csv" file.

## Installation Process

* **Python:** The base language used for automation Install the latest version of python from `https://www.python.org/downloads/`

* **Pip:** This is a package manager, to install pip go to cmd and run command `py -m pip install`

* **PywinAuto:** This is an automation library, pywinauto is a set of python modules to automate the Microsoft Windows GUI.  To install pywinauto execute the command `pip install pywinauto` also go to the official documentation `https://pypi.org/project/pywinauto/0.5.2/`

* **Locator Tool:** We used swappy to locate elements To install swapy  go to cmd and execute the command `pip install swapy` and go to `https://pypi.org/project/swapy/`

* **Java:** Download the latest version of Java from `https://www.oracle.com/pk/java/technologies/downloads/`

* **Alure Report:** We use alure report to create reporting.. Download the report using the command `pip install allure-pytest` and check the official website `https://allurereport.org/docs/pytest/`

## Execution Process

* **Run the whole project:** Just double click the batch file `run_tests` 

* **Run a specific file:** Make sure that you are on that specific directory and path and add command pytest and file nme `pytest [filename]`