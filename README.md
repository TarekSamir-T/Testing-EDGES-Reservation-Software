# EDGES Reservation Software - Final Testing Project

## Overview

This project is a **software testing project** focused on the **EDGES Reservation System**, a desktop application written in **C language**.  
The primary objective was to apply comprehensive **unit testing** using the **CUnit framework** and to implement thorough **manual testing strategies** following best practices learned during the Testing Diploma program.

## Project Objective

- Perform **unit testing** on EDGES Reservation Software using the CUnit framework.
- Apply **manual testing techniques** such as:
  - MC/DC Coverage
  - Branch Coverage
  - Statement Coverage
  - Boundary Value Analysis
  - State Transition Testing
- Generate detailed **Test Case Reports**, **Bug Reports**, and a **Test Completion Report**.

## Software Overview

The EDGES Reservation Software manages two types of users:
- **Admin User**: Can register, delete, and manage student accounts; view user information; and oversee course registrations.
- **Normal User (Student)**: Can create accounts, log in, change passwords, view personal information, and reserve courses.

The system is divided into key components:
- **APP**: Main application runner.
- **Backend**: Core application logic.
- **Course Registration Module**: Handling course enrollments.
- **Create Account Module**: Account creation and validation.
- **DB Manager**: CRUD operations on in-memory database.
- **Login Module**: Authentication handling.
- **Security Module**: Admin security token management.
- **Generic Module**: Common data definitions and constants.
- **Tests**: CUnit test suites for different components.
- **Main.c**: Entry point for running the application or tests.

## Technologies Used

- **Programming Language**: C
- **Unit Testing Framework**: CUnit
- **Manual Testing**: Structured manual test design and execution
- **Automation Tools** (if used additionally): Selenium WebDriver, Postman

## Project Structure

├── source/ # Application source code (C) ├── database/ # Database initialization scripts ├── tests/ # CUnit test cases and test suites ├── documentation/ # Project reports and documentation ├── README.md # Project overview and setup instructions


## Setup Instructions

### 1. Build the Application

Compile the source code using a C compiler:

```bash
gcc main.c -o reservation_system
2. Running the Application
To run the main application:

Keep the Application Run section enabled in Main.c

To run the CUnit Tests:

Comment out the Application section and uncomment the Testing Run section in Main.c

Then execute the compiled test binary.

3. Database Initialization
The software initializes the database with 3 default users upon first run.

Database updates dynamically during session operations.

Testing Strategy
Unit Testing
Developed using the CUnit framework.

Test cases designed to achieve:

MC/DC Coverage

Branch Coverage

Statement Coverage

Manual Testing
Manual test cases cover:

State Transition Testing

Boundary Value Analysis

Functional Requirements Validation

Manual test execution documented with:

Test Inputs, Expected Results, Actual Results

Prerequisites and Techniques Used

Bug Reports (if defects were found)

Deliverables
Updated source code including unit tests.

Test Case Reports for all test cases.

Bug Reports for identified issues.

Test Completion Report detailing coverage and overall testing results.

Important Notes
Admin Login Token: 10203040 (modifiable in Sec.h)

Sample Users:

AdminUser1 / Edges123

AdminUser2 / Edges123456

AdminUser3 / Edges_123

The system database persists across operations during a session.

License
This project is submitted as part of the Testing Diploma program and is governed by training academic policies.

