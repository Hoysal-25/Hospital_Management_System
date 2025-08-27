# 🏥 Hospital Management System

A **Java + JDBC + MySQL** based system to manage hospital operations. The system includes modules for **Doctors**, **Patients**, and **Appointments** with full CRUD functionality and scheduling logic.


## 📌 Features

* **Doctor Management**

  * Add, update, delete, and view doctor records
  * Store specialization and availability

* **Patient Management**

  * Add, update, delete, and view patient records
  * Maintain patient details and medical history

* **Appointment Management**

  * Book, update, cancel, and view appointments
  * Check doctor availability before booking
  * Maintain doctor-patient relationships

* **Database Integration**

  * MySQL relational schema for patients, doctors, and appointments
  * JDBC used for seamless database connectivity

## 🛠️ Tech Stack

* **Language**: Java (JDK 8 or higher)
* **Database**: MySQL
* **Connectivity**: JDBC

## 📂 Database Schema

* **Doctors Table**

  * `doctor_id`, `name`, `specialization`, `availability`

* **Patients Table**

  * `patient_id`, `name`, `age`, `gender`, `contact`

* **Appointments Table**

  * `appointment_id`, `doctor_id`, `patient_id`, `date`, `time`, `status`


## ⚙️ Installation & Setup

1. **Clone Repository**

   ```bash
   git clone https://github.com/yourusername/HospitalManagementSystem.git
   cd HospitalManagementSystem
   

2. **Set Up Database**

   * Create a database in MySQL:

     sql
     CREATE DATABASE hospital_db;
     
   * Import the schema (provided in `/database/schema.sql`)

     sql
     USE hospital_db;
     SOURCE schema.sql;
     

3. **Configure JDBC Connection**

   * Update your database credentials in the Java file:

     java
     String url = "jdbc:mysql://localhost:3306/hospital_db";
     String user = "root";
     String password = "yourpassword";
     

4. **Compile & Run**

   bash
   javac -cp .:mysql-connector-java.jar HospitalManagementSystem.java
   java -cp .:mysql-connector-java.jar HospitalManagementSystem
  

## 🎯 Usage

* Run the program and select from the menu:

  * Manage Patients
  * Manage Doctors
  * Book/View Appointments

## 🚀 Future Enhancements

* GUI with **Java Swing/JavaFX**
* Role-based authentication (Admin, Doctor, Patient)
* Prescription & billing module
* REST API integration

## 🤝 Contributing

Contributions are welcome! Please fork the repo and submit a pull request.


## 📜 License

This project is licensed under the **MIT License** – feel free to use it.


Would you like me to also **generate a `schema.sql` file** for the MySQL database (with `CREATE TABLE` statements) so that you can include it in your repo?
