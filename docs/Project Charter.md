Software Requirements Specification

# ETL Support

## Software Requirements Specification for Team 2
### Version 1.0

## Table of Contents
### 1) Introduction
- Overview
- Goals and Objectives
- Scope

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
### Overview
The ETL-Support program will be a Python script available only for Windows operating system. The program will allow you to back up your classroom reservation management data on a server (SIGMAQ). The backup result will be made available by the Reporting Service of the school.
This document provides information on the requirements for the ETL Support software application.

### Goals and Objectives
The purpose of ETL Support is to back up classroom reservation time data on a server (SIGMAQ) to allow for the visualization of the data thanks to the reporting services of the school.

### Scope
As per introduction, the purpose of the program is to back up class booking data and to allow a visualization of the data to the reporting service of the school.

### Definitions
- *Stackholder:* It's the person who's part of the process ETL-Support.

## 2) General Design Constraints 

### ETL-Support Application Environment