Software Requirements Specification

# ETL Support

## Software Requirements Specification for Team 2
### Version 1.0
### Document Owner: Elia Vicentini

## Table of Contents
### 1) Introduction
- Overview
- Goals and Objectives
- Scope
- Definitions

### 2) General Design Constraints
- ETL Support Application Environment
- User Characteristics
- Mandated Constraints

### 3) Nonfunctional Requirements
- Operational Requirements
- Performance Requirements
- Security Requirements
- Documentation and Training
- External Interface
    - User Interface
    - Software Interface

### 4) Functional Requirements
- Required Features
- Optional Features

## Revision History
|Version    |Date       |Name   |Description                                |
|-----------|-----------|-------|-------------------------------------------|
|1          |29/03/2019 |       |Pianificazione exportdata.py               |  
|2          |29/03/2019 |       |Creazione file di configurazione json      |  
|3          |30/03/2019 |       |Produzione setup.py                        |  
|4          |02/04/2019 |       |Creazione exportdata.py                    |  
|5          |02/04/2019 |       |Tests                                      |  
|6          |02/04/2019 |       |Bug fixes                                  |  
|7          |03/04/2019 |       |Progettazione script per i file di log     |  
|8          |04/04/2019 |       |Completata la prima versione del programma |  
|9          |20/09/2019 |       |Update exportdata.py                       |  
|10         |30/09/2019 |       |Bug fixes                                  |  
|11         |30/09/2019 |       |Update all scripts                         |  
|12         |21/10/2019 |       |Completato lo script per i file di log     |  
|13         |16/12/2019 |       |Perfezionamento di exportdata.py           |  
|14         |16/12/2019 |       |Completata la versione finale del programma|

## 1) Introduction

### 1.1) Overview
The ETL-Support program will be a Python script available only for Windows operating system. The program will allow you to back up your classroom reservation management data on a server (SIGMAQ). The backup result will be made available by the Reporting Service of the school.
This document provides information on the requirements for the ETL Support software application.

### 1.2) Goals and Objectives
The purpose of ETL Support is to back up classroom reservation time data on a server (SIGMAQ) to allow for the visualization of the data thanks to the reporting services of the school.

### 1.3) Scope
As per introduction, the purpose of the program is to back up class booking data and to allow a visualization of the data to the reporting service of the school.

### 1.4) Definitions
- *Stackholder:* It's the person who's part of the process ETL-Support.

## 2) General Design Constraints 

### 2.1) ETL-Support Application Environment
The ETL-Support program includes a CLI application that only works on the Windows operating system. There is no GUI.

### 2.2) User Characteristics
The application is not intended to be used by many users, but only by one, the stackholder of the ETL-Support project, Professor Gianni Bellini.

### 2.3) Mandated Constraints
The application will only work on the Windows operating system. The reason for this choice is due to the use of libraries to connect to an SQL Server, the latter also produced by Microsoft.

## 3) Nonfunctional Requirements

### 3.1) Operational Requirements
Usability: All those who will use the program will not need to read the documentation, just enter a command to start it all.

### 3.2) Performance Requirements
Compatibility: For greater compatibility with the operating system, we recommend using the program with the help of a Python Virtual Environment and installing the libraries within it.

### 3.3) Security Requirements
The ETL-Support program does not have any security features

### 3.4) Documentation and Training
The ETL-Support program will be delivered to the stackholder via the GitHub platform. There will be no documentation attached to the program.

### 3.5) External Interface

### 3.5.1) User Interface 
The application is presented through a CLI interface, all the steps of the program will be clear and intuitable by those who will use it

### 3.5.2) Software Interface
The application will interface with three servers:
- *edu-x04* (MySQL Server)
- *edu-x08* (API MarconiTT)
- *edu-sys01* (SIGMAQ)
The first two servers can be chosen when the program starts.

## 4) Functional Requirements

### 4.1) Required Features

### 4.1.1) Use Case: direct
**Description:** Direct connection to edu-x04
Actor: Stackholder

Command: **exportdata.py direct**

### 4.1.2) Use Case: api
**Description:** Connection to edu-x08 via MarconiTT API
Actor: Stackholder

Command: **exportdata.py api**

## 4.2) Optional Features

### 4.2.1) Use Case: Change MySQL or SQLServer
**Description:** Possibility to change MySQL Server or SQL Server
Actor: Stackholder

Command example: **exportdata.py direct mysql-x04 sql-garuda63**