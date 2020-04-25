
# ETL - Support
# Iteration Plan

___
## **ETL Support 2019 - Group 2**

<br>

## Team Members

- Elia Vicentini (Scrum Master)
- Simone Gandini
- Luca Landolfo
- Enrico Marocchio
- Adrian Munteanu 

<br>

### **Document Owner**

Luca Landolfo is responsible for the development and maintenance of this document.
___
<br>
<br>

## Iteration #1
_29/03/19 - 04/04/19_

### Revision History

<br>

| Author | Date | Description |
|--|--|--|
| Elia Vicentini | 29/03/19 | Initial release. |
| Luca Landolfo | 29/03/19 | Added JSON connection file. |
| Luca Landolfo | 29/03/19 | Connect to the server via JSON's data. |
| Elia Vicentini | 30/03/19 | Added 'PyMySQL' library. |
| Luca Landolfo | 30/03/19 | Implemented boold. |
| Elia Vicentini & Adrian Munteanu | 30/03/19 | Created setup.py |
| Enrico Marocchio | 30/03/19 | Created logcreator.py |
| Whole Tean | 31/03/19 | Various updates to work with a test server. |
| Adrian Munteanu & Simone Gandini | 01/04/19 | Improved different functions. |
| Luca Landolfo & Elia Vicentini| 01/04/19 | Connection to edu-x04 and 1° query execution. |
| Whole Tean | 02/04/19 | Updates on the logging and errors exception functionalities. |
| Elia Vicentini & Luca Landolfo | 03/04/19 | Added functionality to insert data into the database.  |
| Luca Landolfo, Adrian Muntanu & Simone Gandini | 03/04/19 | Added sys-argv and improved several minor errors. |
| Enrico Marocchio | 03/04/19 | Updated and added more functionalities for the logging system. |
| Enrico Marocchio | 04/04/19 | Completed logcreator.py. |

<br>

## Objectives
The main purpose of this initial iteration is to plan and create a first working prototype of the python script. It must be able to connect and perform the first simple operations on the databases, efficiency it's not required. It was also requested to implement a logging system, in order to make the whole process more understandable, especially in case of mistakes.
At the end of this first iteration the system should be able to:
- Connect to the server through data provided by a json file.
- Taking, processing and returning data from a database to a newer one.
- Have a simple and user-friendly GUI (even if from CLI).
- Save every process executed by the program on a .log file.

<br>

___
<br>
<br>

## Iteration #2
_20/09/19 - 16/12/19_

### Revision History

<br>

| Author | Date | Description |
|--|--|--|
| Elia Vicentini | 20/09/19 | Added 'requests' library. |
| Enrico Marocchio | 20/09/19 | Updated .log file visuals. |
| Whole Team | 21/09/19 | Save API data on a .csv file and process it. |
| Luca Landolfo & Elia Vicentini | 23/09/19 | Improved queries performance and simplified the query process. |
| Elia Vicentini | 27/09/19 | Other queries improvements and added boolsql. |
| Whole Team | 28/09/19 | Various updates and fixes to work with the DB. |
| Elia Vicentini | 07/10/19 | Updated print and config messages. |
| Enrico Marocchio & Elia Vicentini | 21/10/19 | Updated logcreator to work with both API and Direct modes. |
| Whole Team | 16/12/19 | Fixed and improved some parameters for MySQL and SQL server. |
| Whole Team | 16/12/19 | Script fully completed and working. |

<br>

## Objectives
This version of code will first have to work with MarconiTT's API to connect to the server and the databases. Obviously the connection method of the last iteration will have to work without problems anyway. The program will also need to be much more efficient and for this reason it will mainly be necessary to change the queries that are executed on the database.
At the end of this iteration the system should be able to:
- Rework the whole app to work with the API.
- Connect to the API and grab the data needed provided by the API.
- Save, process and enter data into the target database.
- Greatly improve the processing and uploading of data from .csv files to the SQL server via queries.
- Recognize and fix all the faults in the code.

