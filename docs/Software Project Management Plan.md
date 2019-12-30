# Software Project Management Plan
## **ETL Support 2019 - Group 2**
### _January 7, 2019_

<br>

## **Team Members**

- Elia Vicentini (Scrum Master)
- Simone Gandini
- Luca Landolfo
- Enrico Marocchio
- Adrian Munteanu
 

### **Document Storage**

This document is stored in a GitHub [repository](https://github.com/IlVice26/GPI-Documents-Group2.git), where you can also find all the other types of documentation regarding this project.

  

### **Document Owner**

Luca Landolfo is responsible for the development and maintenance of this document.

  

<br>

  

# Table of Contents

### **1 OVERVIEW**
1.1 Purpose and Scope
1.2 Goals and Objectives
1.3 Project Deliverables 
1.4 Assumptions and Constraints
1.5 Success Criteria
1.6 Definitions
### 2 STARTUP PLAN
2.1 Team Organization
2.2 Project Communications
2.3 Technical Process
2.4 Tools

# 1. Overview

## 1.1 Purpose and Scope
The team behind ETL has the task of providing a script to **manage, modify, update and provide a backup plan,** for the data obtained from another project in our working environment, MarconiTT, a web application.

This script has the task of speeding up, supporting and updating the data needed throughout the web app process.  

The script, written entirely in _Python 3.7_, communicates and works with different _SQL_ databases within the work environment by **moving, deleting and updating** data from one database to another.

You will need to start the Script via any shell, from _cmd_ (Windows) to any _Linux_ or _OSX_ command prompt.
You will be able to start the program in _two_ different ways: 

 - **direct**
	 - The program will connect **directly** to the school's main database in order to work faster.
 - **api**
	 - The program will connect to the school's database **via an API**, specifically created by the MarconiTT team.

The program will be used primarily by the authorized stakeholder: _**Prof. Bellini G.**_

## 1.2 Goals and Objectives
The goal is to provide a functional and fast script, for a better management and reliability of the **data concerning the school's classroom reservations**, which will then be used by the MarconiTT web application for a better visualization of the data.

**Project Goals and Objectives:**
 1. Create an app that is as fast as possible in calculations and simple to use.
 2. Speed up the process behind the school's classroom reservations.
 3. Provide correct and reliable data to the MarconiTT team.
 4. Learn more about SQL, Databases and Python.

## 1.3 Project Deliverables
| Date | Deliverable |
|--|--|
| 29/03/2019 | Plan _exportdata.py_ |
| 29/03/2019 | json configuration file creation |
| 30/03/2019 | Production _setup.py_ |
| 02/04/2019 | Prototype of _exportdata.py_ |
| 02/04/2019 | Tests | 
| 02/04/2019 | Bug fixes |
| 03/04/2019 | Script design for log files |
| 04/04/2019 | Completed the first version of the program |
| 20/09/2019 | Update _exportdata.py_ |
| 30/09/2019 | Bug fixes |
| 30/09/2019 | Update all scripts |
| 21/10/2019 | Finished the script for log files |
| 16/12/2019 | Improvement of _exportdata.py_ |
| 16/12/2019 | Finished the final version of the product |

## 1.4 Assumptions and Constraints
 - _**Assumptions**_
	 - The data is already correct, available and easily accessible.
	 - The machine on which the program will be started already owns Python 3.7.
	 - That all databases are available and connected.
 - _**Constraints**_
	 - Stakeholder approval required for the execution of SQL queries.
	 - Can only work at school.
	 - Not much time.

## 1.5 Success Criteria
Creation of a working, secure and fast running script, runnable everywhere and easy to use, that not only updates the data on the different databases, but also backs them up in case something goes wrong.

## 1.6 Definitions
| Term | Definition |
|--|--|
| Actor | User or other software system that receives value from a user case |
| Developer | The person or team who is developing the application |
| Scenario | One path through a user case |
| Stakeholder | Anyone of the entities directly or indirectly involved in the project and its outcomes |
| User | The person or group of people that will actually use with the application |
| User case | Describes how an actor will perform tasks on the system. It may define many different variants called scenarios that can lead to different outcomes. |


# 2 Startup Plan

## 2.1 Team Organization

| Role | Actor(s) | Responsibility |
|--|--|--|
| Scrum Master | Vicentini | Responsible for managing and coordinating the exchange of information between team members, also assign tasks to teammates. |
| Developer | Landolfo, Vicentini, Munteanu, Marocchio, Gandini | Write the software based on requirement and architect specifications |
| Tester | Gandini, Landolfo | Test the code, report issues, find and fix bugs, work on the code's efficiency |
| Architect | Vicentini | Specify overall internal workings of application |
| Requirement Engineer | Munteanu, Landolfo, Vicentini | Define, document and keep track of the requirements |

## 2.2 Project Communications

| Event | Information | Audience | Format | Frequency |
|--|--|--|--|--|
| Team Meeting | Task status: what has been completed since last meeting and what were the problems encountered; planning on what's next. | All team members | Informal meetings before working; Messages for status updates and problems as they occur. | As needed |
| Project Status Report | Review of the sprint, status of the prototype, coding issues, problems relating the project | All team members, Stakeholder | Informal meetings before working | Iteration Closeout |

## 2.3 Technical Process

Planned an incremental development process. The first iterations will be to lay the groundwork on what we need. Subsequent iterations will mostly work on the actual data.
Feedback from the Stakeholder will be used to improve the next iteration.

## 2.4 Tools

 - _Programming Languages_ - Python, SQL
 - _Operating System_ - Windows
 - _Version Control System_ - Git, the project will be stored on a GitHub repository
 - _Development Tools_- Visual Studio Code, SQL Server

 
