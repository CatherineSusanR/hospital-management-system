
# 🏥 Hospital Management System – Database

This repository contains the complete **SQL schema** for a Hospital Management System. It defines the core tables and relationships required to manage users, doctors, patients, appointments, billing, and insurance.

---

## 📦 Database Files

- `hospitaldb_users.sql` – Contains login credentials for hospital system users.
- `hospitaldb_doctors.sql` – Stores doctor profiles and details.
- `hospitaldb_patients.sql` – Manages patient personal and medical information.
- `hospitaldb_appointments.sql` – Tracks appointments between patients and doctors.
- `hospitaldb_billing.sql` – Manages patient billing and payment records.
- `hospitaldb_insurance.sql` – Stores information about patient insurance policies.

---

## 📌 Features

- 👤 **User Management**  
  Handles authentication and access for hospital staff.

- 🧑‍⚕️ **Doctor Management**  
  Stores doctor names, specializations, contact info, and more.

- 🧍 **Patient Records**  
  Tracks demographics, medical history, and visit history.

- 📅 **Appointments**  
  Links doctors and patients for scheduled consultations.

- 💵 **Billing System**  
  Records charges, payments, and bill status.

- 🛡️ **Insurance Info**  
  Keeps insurance provider details tied to patient records.

---

## ⚙️ How to Set Up

### 1. Create the Database

Open your MySQL terminal or preferred database tool:

```sql
CREATE DATABASE hospital_db;
USE hospital_db;
````

### 2. Import SQL Files (in order)

Run each command below to import the tables:

```bash
mysql -u root -p hospital_db < hospitaldb_users.sql
mysql -u root -p hospital_db < hospitaldb_doctors.sql
mysql -u root -p hospital_db < hospitaldb_patients.sql
mysql -u root -p hospital_db < hospitaldb_appointments.sql
mysql -u root -p hospital_db < hospitaldb_billing.sql
mysql -u root -p hospital_db < hospitaldb_insurance.sql
```

> ⚠️ **Import in this order** to avoid foreign key constraint issues.

---

## 🗃️ Example Structure (ER Overview)

Although the ER diagram isn't included, the general relationships are:

* `users` – Handles system authentication
* `doctors` ↔ `appointments` ↔ `patients` – Manages consultations
* `patients` ↔ `billing` – Tracks financials
* `patients` ↔ `insurance` – Links insurance details

---

## 👩‍💻 Author

**Catherine Susan**
📍 [GitHub](https://github.com/CatherineSusanR) • [LinkedIn](https://in.linkedin.com/in/catherine-susan-rajesh-53686b2b4) • [Instagram](https://instagram.com/catherinesuzn)

---

## 📝 License

This project is open-source and available under the MIT License.

```

