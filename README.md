# Project Title: Library Management System

## Description

This project implements a database management system for a library, using MySQL. It allows you to manage information about authors, categories, books, members, loans, and reservations.  This system provides a structured way to organize and track library resources and member activities.

## Features

* **Author Management:** Store author details including name, birth date, and nationality.
* **Category Management:** Organize books into categories (e.g., Fiction, Non-Fiction).
* **Book Management:** Maintain a catalog of books with titles, ISBNs, publication dates, and publishers.
* **Member Management:** Keep track of library member information, including contact details and membership dates.
* **Loan Management:** Record book loans to members, including loan and return dates.
* **Reservation Management:** Handle book reservations by members.
* **Database Structure:** A relational database design with tables and relationships to ensure data integrity and efficient querying.

## How to Run/Set Up the Project

1.  **Prerequisites:**
    * MySQL Server installed and running.
    * A MySQL client (e.g., MySQL Workbench, Dbeaver, or the MySQL command-line tool).

2.  **Installation:**
    * Clone this repository to your local machine.
    * Open your MySQL client.
    * Create a new database (e.g., `library_db`):
        ```sql
        CREATE DATABASE library_db;
        USE library_db;
        ```
    * Import the SQL schema:
        * Using the MySQL command-line tool:
            ```bash
            mysql -u your_username -p library_db < library_management_system.sql
            ```
        * Using MySQL Workbench or Dbeaver:
            * Connect to your MySQL server.
            * Select the `library_db` schema.
            * Open the `library_management_system.sql` file.
            * Execute the script to create the tables.

3.  **Database Schema:**
    The database schema consists of the following tables:
    * `author`
    * `category`
    * `book`
    * `book_author` ( связующая таблица)
    * `member`
    * `loan`
    * `reservation`

 

## Repository Contents

The repository includes the following:

* `library_management_system.sql`:  The SQL script to create the database schema (tables, relationships, and constraints).
* `README.md`: This file, providing project information and setup instructions.
