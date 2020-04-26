# Test Case Specification

## ETL - Support 2019 - Group 2

### Team Members

-   Elia Vicentini (Scrum Master)
-   Simone Gandini
-   Luca Landolfo
-   Enrico Marocchio
-   Adrian Munteanu

### Document Owner

Adrian Munteanu is responsible for the development and maintenance of this document.

### Introduction

This document provides the test cases to be carried out for the ETL-Support-2019 Application. Each item to be tested is represented by an individual test case.  Each case details the input and expected outputs.

---

### Revision History

||||
|-|-|-|
|Author|Date|Description|
|Elia Vicentini|29/03/19|Initial release.|
|Luca Landolfo|29/03/19|Added JSON connection file.|
|Luca Landolfo|29/03/19|Connect to the server via JSON's data.|
|Elia Vicentini|	30/03/19|	Added 'PyMySQL' library.|
|Luca Landolfo|	30/03/19|	Implemented boold.|
|Elia Vicentini & Adrian Munteanu|	30/03/19|	Created `setup.py`|
|Enrico Marocchio|30/03/19|	Created `logcreator.py`|
|Whole Team|	31/03/19|	Various updates to work with a test server.|
|Adrian Munteanu & Simone Gandini|	01/04/19|	Improved different functions.|
|Luca Landolfo & Elia Vicentini|	01/04/19|	Connection to edu-x04 and 1° query execution.|
|Whole Team|	02/04/19|	Updates on the logging and errors exception functionalities.|
|Elia Vicentini & Luca Landolfo|	03/04/19|	Added functionality to insert data into the database.|
|Luca Landolfo, Adrian Muntanu & Simone Gandini|	03/04/19|	Added sys-argv and improved several minor errors.|
|Enrico Marocchio|	03/04/19|	Updated and added more functionalities for the logging system.|
|Enrico Marocchio|	04/04/19|	Completed `logcreator.py`|

---

### Test Cases

|||
|-|-|
|Test Case ID:|1.1|
|Title:|Write data on CSV file from MySQL DataBase|
|Feature/Sub-feature:|Application arguments|
|Purpose:|To ensure that it is possible to connect to MySQL server and the data is being saved on CSV file.|
|Test Data:|Test Data will include info taken from MySQL DataBase|
|Test Actions:|1. Open cmd <br /> 2. Run the `exportdata.py` with `--mode direct` and `--noupload` (to do not insert any data) as arguments|
|Expected Results:|After Step 2 a CSV file named `database-direct.csv` should appear in the folder with no errors.|

---

|||
|-|-|
|Test Case ID:|1.2|
|Title:|Write data on CSV file from API|
|Feature/Sub-feature:|Application arguments|
|Purpose:|To ensure that it is possible to connect to API and the data is being saved on CSV file.|
|Test Data:|Test Data will include info taken from API|
|Test Actions:|1. Open cmd <br /> 2. Run the `exportdata.py` with <br /> `--mode api` and `--noupload` (to do not insert any data) as arguments|
|Expected Results:|After Step 2 a CSV file named `database-api.csv` should appear in the folder with no errors.|

---

|||
|-|-|
|Test Case ID:|1.3|
|Title:|Log file|
|Feature/Sub-feature:|Logs|
|Purpose:|To assure that all actions are tracked in the log file|
|Test Data:|Test Data will include info taken from any source (MySQL server or API)|
|Test Actions:|1. Open cmd <br /> 2. Run the `exportdata.py` in any mode and `--noupload` (to do not insert any data) as argument|
|Expected Results:|After Step 2 a log file named `exportadata_CURRENTDATE.log` should appear in the `log` folder with no errors.|

---

|||
|-|-|
|Test Case ID:|1.4|
|Title:|Insert data into MySQL DataBase|
|Feature/Sub-feature:|Application arguments|
|Purpose:|To make sure that it is possible to connect to MySQL server and insert data|
|Test Data:|Test Data will include info taken from any source (API or direct)|
|Test Actions:|1. Open cmd <br /> 2. Run the `exportdata.py` in any mode and with `--mysql` as argument|
|Expected Results:|After Step 2 data from CSV file should be inserted in the MySQL DataBase with no errors.|

---

|||
|-|-|
|Test Case ID:|1.5|
|Title:|Insert data into SQL DataBase|
|Feature/Sub-feature:|Application arguments|
|Purpose:|To make sure that it is possible to connect to SQL server and insert data|
|Test Data:|Test Data will include info taken from any source (API or direct)|
|Test Actions:|1. Open cmd <br /> 2. Run the `exportdata.py` in any mode and with `--sql` as argument|
|Expected Results:|After Step 2 data from CSV file should be inserted in the SQL DataBase with no errors.|

---

|||
|-|-|
|Test Case ID:|1.6|
|Title:|Insert data into SQL DataBase|
|Feature/Sub-feature:|Application arguments|
|Purpose:|To make sure that it is possible display additional details about what the program is doing|
|Test Data:|Test Data will include info taken from any source (API or direct)|
|Test Actions:|1. Open cmd <br /> 2. Run the `exportdata.py` in any mode with `--noupload` (to do not insert any data) and `-v` as arguments|
|Expected Results:|After Step 2 details about what the program is doing should be displayed in the cmd.|
