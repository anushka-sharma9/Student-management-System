# **Student Management System** 🎓
A robust **Student Management System** built using **Python (Tkinter)** and **MySQL**, designed to streamline student data management with an intuitive graphical user interface.  

---

## **Project Overview**  
This project allows users to efficiently manage student records, including adding, viewing, updating, and deleting entries. It's an excellent example of integrating Python-based GUI applications with a backend database.  

---

## **Repository Contents**  

1. **`main.py`**:  
   - The main script containing the implementation of the student management system.  
   - It handles GUI design, user interactions, and integrates database connectivity for CRUD (Create, Read, Update, Delete) operations.  
   - Uses **Tkinter** for the GUI and **pymysql** for MySQL database communication.  

2. **`custom.py`**:  
   - A configuration file defining UI customization settings such as colors and fonts.  
   - Ensures consistent design aesthetics across the application.  
   - Variables like `color_1`, `font_1`, etc., are imported and used in `main.py`.  

3. **`credentials.py`**:  
   - Contains sensitive database connection details like:
     - `host`  
     - `user`  
     - `password`  
     - `database`  
   - Ensures modularity and easy updates for database credentials without modifying the core application logic.  
   - **Important**: Add this file to `.gitignore` to prevent exposing sensitive information.  

4. **`LICENSE`**:  
   - Defines the licensing terms under which this project can be used.  
   - This repository uses the **MIT License**, allowing others to freely use, modify, and distribute the code with proper attribution.  

---

## **Features**  
- Add, view, update, and delete student records.  
- Database integration ensures persistent storage.  
- Simple and user-friendly GUI.  

---

## **Tech Stack**  
- **Programming Language**: Python  
- **Framework**: Tkinter (for GUI)  
- **Database**: MySQL  
- **Libraries**:  
  - `pymysql` for database operations  
  - `functools` for efficient code management  

---

## **Setup Instructions**  

1. **Clone the Repository**:  
   ```bash
   git clone https://github.com/username/student-management-system.git
   cd student-management-system
   ```
2. **Install Dependencies**:  
   ```bash
   pip install pymysql
   ```
3. **Set Up MySQL Database**:  
   - Create a database named `student_management`.  
   - Run the following SQL command to create the required table:  
     ```sql
     CREATE TABLE student_register (
       f_name VARCHAR(50),
       l_name VARCHAR(50),
       course VARCHAR(50),
       subject VARCHAR(50),
       year INT,
       age INT,
       gender VARCHAR(10),
       birth DATE,
       contact VARCHAR(15) PRIMARY KEY,
       email VARCHAR(100)
     );
     ```
4. **Update Database Credentials**:  
   - Open `credentials.py` and update it with your MySQL credentials:  
     ```python
     host = '127.0.0.1'
     user = 'your-username'
     password = 'your-password'
     database = 'student_management'
     ```
5. **Run the Application**:  
   ```bash
   python main.py
   ```

---

## **Future Enhancements**  
- Adding search functionality.  
- Exporting student records to CSV or Excel.  
- Enhanced validation for input fields.  

---


