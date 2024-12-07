# Health Care Management System

## Overview
The **Health Care Management System** is a C program that helps manage patient records, BMI calculations, blood donation information, step count analysis, and event organization. It features interactive menus and data persistence through file storage.

---

## Features
### 1. **BMI Calculation**
   - Calculates BMI based on user-provided height and weight.
   - Displays health status using a BMI scale.

### 2. **Step Count Analysis**
   - Converts distance walked (in kilometers) to steps.
   - Compares steps to a target (8,000 steps) and provides feedback on target fulfillment.

### 3. **Patient Information Management**
   - Add and display patient records.
   - Calculates BMI for each patient based on height and weight.

### 4. **Blood Donation Management**
   - Add, delete, display, and search blood donation records.
   - Supports search by blood type, location, and mobile number.

### 5. **Event Management**
   - Add, delete, and display upcoming health-related events.

### 6. **Data Persistence**
   - Saves and loads data (patients, events, and blood donations) to/from a file (`health_records.txt`).

### 7. **Developer Information**
   - Displays information about the development team.

---

## How to Use
### Compilation
Use the following command to compile the program:
```bash
gcc -o health_care_management health_care_management.c -lm
```

### Running the Program
Run the compiled program:
```bash
./health_care_management
```

### Navigation
The program offers a main menu with the following options:
- **1. Calculate BMI**
- **2. Calculate Step Count**
- **3. Patient Information**
  - Add or display patient records.
- **4. Blood Donation Information**
  - Add, delete, display, or search blood donation records.
- **5. Events**
  - Add, delete, or display events.
- **6. Exit**
  - Saves data to file and exits the program.
- **7. About Developers**
  - Displays information about the development team.

---

## Code Details
### Data Structures
- **`struct Patient`**
  - Stores patient information (name, age, height, weight, BMI).
- **`struct Event`**
  - Stores event information (name, date, place).
- **`struct DonationInfo`**
  - Stores blood donation details (donor name, blood type, date, location, mobile number).
- **`struct StackNode`**
  - Implements a stack for managing blood donation records.

### Key Functions
- **Patient Management**
  - `createPatient()`, `insertPatient()`, `displayPatients()`
- **BMI Calculation**
  - `calculateBMI()`
- **Step Count**
  - `calculateStepCount()`
- **Blood Donation Management**
  - `createDonationInfo()`, `push()`, `pop()`, `display()`, `searchAndDisplay()`
- **Event Management**
  - `createEvent()`, `pushEvent()`, `popEvent()`, `displayEvents()`
- **File Operations**
  - `saveToFile()`, `loadFromFile()`

---

## Data Persistence
Data is saved in `health_records.txt` in the following format:
- **Patients:** `Patient <name> <age> <height> <weight> <bmi>`
- **Events:** `Event <name> <date> <place>`
- **Blood Donors:** `Donor <name> <blood_type> <date> <location> <mobile_number>`

---

## Requirements
- GCC compiler.
- Terminal or console for program execution.

---

## Developers
- **Team Falcons**
  - Mitin Deb Rudro (Project Administrator)
  - Durjoy Das (Database Administrator)
  - Adhora Madhuri (Web Manager)
  - Swity Saima (Software Designer)
  - MD. Arrafiu Akash (Quality Assurance)

---
