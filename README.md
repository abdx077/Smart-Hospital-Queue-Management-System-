
# HospitalFlow IQ
### Smart Multi-Department Hospital Patient Flow, Referral & Resource Optimization System

---

## 1. Project Overview

HospitalFlow IQ is a C++ based hospital management system designed to organize patient registration, department management, doctor assignment, queue handling, and interdepartmental referrals.

The system aims to improve hospital workflow by maintaining patient visit history, estimating waiting times, monitoring department workload, and helping hospital staff manage patient flow more efficiently.

It provides a centralized, menu-driven console application where different authorized users can perform operations according to their roles.

## 2. Project Objectives

- Organize patient registration and record management.
- Maintain patient medical visit history.
- Manage multiple hospital departments independently.
- Improve patient queue organization.
- Support interdepartmental referrals.
- Monitor doctor availability and workload.
- Estimate patient waiting times.
- Identify overcrowded departments.
- Analyze hospital traffic and workload statistics.
- Simulate the possible impact of adding hospital staff.

## 3. Main Features

### 3.1 Patient Management
- Register new patients.
- Generate unique Patient IDs.
- Search and update patient records.
- Maintain individual patient information.

### 3.2 Patient Medical History
- Retrieve previous patient visits.
- Maintain separate Visit IDs for each encounter.
- View previous departments, complaints, referrals, and visit outcomes.
- Generate repeat complaint alerts for staff review.

### 3.3 Smart Department Recommendation
- Accept patient complaints in text form.
- Use keyword-based matching to suggest a relevant department.
- Support multiple complaint keywords and patterns.
- Allow authorized staff to confirm the suggested department.

### 3.4 Multi-Department Queue Management
- Manage separate queues for hospital departments.
- Generate patient tokens.
- Organize patients according to assigned priority.
- Track waiting, served, and pending patients.

### 3.5 Emergency and Priority Handling
- Support emergency, urgent, and normal priority categories.
- Allow authorized staff to assign clinical priority.
- Display appropriate emergency assessment warnings.

### 3.6 Doctor Management
- Register doctors.
- Assign doctors to departments.
- Track doctor availability.
- Monitor individual doctor workload.
- Recommend available doctors based on specialty and workload.

### 3.7 Interdepartmental Referrals
- Transfer patients between departments.
- Generate unique Referral IDs.
- Record referral reasons and requesting departments.
- Track pending, accepted, and rejected referrals.
- Preserve the patient's original visit history.

### 3.8 Waiting Time Estimation
- Estimate waiting time using patients ahead and average consultation duration.
- Display estimated waiting times.
- Help staff monitor patient waiting periods.

### 3.9 Department Workload Monitoring
- Monitor department queues.
- Calculate department workload.
- Display congestion warnings.
- Track registered, waiting, and served patients.

### 3.10 Hospital Traffic Analysis
- Maintain department statistics.
- Calculate average waiting times.
- Analyze daily and historical patient traffic.
- Compare department workload trends.

### 3.11 What-If Staff Addition Simulation
- Simulate adding an additional doctor or staff member.
- Compare estimated waiting times before and after the simulation.
- Help management evaluate possible workload improvements without changing actual records.

### 3.12 File-Based Data Storage
- Store patient records.
- Store doctor information.
- Maintain department information.
- Save visit and referral records.
- Retrieve saved information when the application restarts.

### 3.13 Role-Based Access Control
- Provide separate access for administrators, receptionists, and doctors.
- Restrict operations according to user permissions.
- Protect sensitive patient information from unauthorized access.

## 4. Types of Users

| User Type | Responsibilities |
|---|---|
| Administrator | Manage departments, doctors, users, and hospital statistics. |
| Receptionist | Register patients, search records, and manage patient queues. |
| Doctor | View authorized patient history, manage consultations, and create referrals. |

## 5. Technologies Used

### Programming Language
- C++

### Development Environment
- Visual Studio Code
- GCC / MinGW C++ Compiler

### Core C++ Concepts
- Variables and Data Types
- Input and Output Operations
- Conditional Statements (if, if-else, switch)
- Loops (for, while, do-while)
- One-Dimensional Arrays
- Two-Dimensional Arrays
- Structures (struct)
- Nested Structures
- Functions and Function Prototypes
- Recursion
- Pointers and Dereferencing
- References
- Pointer Arithmetic
- Passing Arguments by Value and Reference
- Functions with Arrays
- Functions with Pointers
- String Handling and String Operations

### File Handling and Data Management
- File Input and Output (fstream)
- Reading and Writing Text Files
- Data Persistence
- Record Searching and Updating

### System Development Concepts
- Modular Programming
- Menu-Driven Console Interface
- Role-Based Access Control
- Queue Management Logic
- Priority-Based Patient Handling
- Waiting Time Estimation
- Statistical Calculations
- Keyword-Based Department Recommendation
- What-If Simulation

### Version Control and Documentation
- Git
- GitHub
- README Documentation

## 6. Proposed Project Structure

The application will be organized into logical modules:

- main.cpp — Main program and menu system
- patients.cpp — Patient registration and management
- doctors.cpp — Doctor management and assignment
- departments.cpp — Department management
- queues.cpp — Patient queue operations
- referrals.cpp — Interdepartmental referrals
- history.cpp — Patient medical history
- analytics.cpp — Workload and traffic analysis
- storage.cpp — File handling and data persistence

The final file organization may change during development.

## 7. Working Process

1. Administrator configures hospital departments and doctors.
2. Receptionist registers a new patient or searches for an existing patient.
3. The system retrieves previous visit history when available.
4. The patient's complaint is entered.
5. The system suggests a relevant department using keyword matching.
6. Authorized staff confirms the department and priority.
7. The patient receives a queue token.
8. The system estimates waiting time and monitors department workload.
9. The doctor handles the consultation and records the visit outcome.
10. If necessary, the doctor creates a referral to another department.
11. The receiving department processes the referral.
12. Hospital management can review statistics and run staff addition simulations.

## 8. Data Storage

The system is planned to use text files for persistent storage:

- patients.txt
- doctors.txt
- departments.txt
- visits.txt
- referrals.txt
- users.txt

This allows information to remain available after the application is closed and restarted.

## 9. Project Limitations

- The project is a C++ console-based academic prototype.
- Department recommendations use keyword matching rather than artificial intelligence.
- Waiting time calculations are estimates, not guaranteed service times.
- The system does not provide medical diagnoses or prescriptions.
- Clinical priorities and referral decisions remain under authorized medical staff.
- File-based storage is intended for an academic demonstration, not production hospital deployment.

## 10. Future Scope

- Graphical User Interface (GUI).
- Database integration.
- Web-based hospital access.
- Advanced reporting and visualization.
- More sophisticated patient traffic forecasting.
- Secure authentication and improved access management.

## 11. Academic Information

**Institution:** Ghulam Ishaq Khan Institute of Engineering Sciences and Technology (GIKI)

**Department:** Computer Science

**Course:** CS-101

**Semester:** Fall 2026

**Project:** HospitalFlow IQ

## 12. Project Status

Currently under development as a CS-101 semester project.

Implementation, testing, and documentation will be updated as development progresses.

---

## Disclaimer

HospitalFlow IQ is an educational software prototype developed for academic purposes. It is not intended to replace professional medical judgment, clinical diagnosis, or real hospital management infrastructure.
