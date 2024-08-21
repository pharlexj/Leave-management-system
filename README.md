# Leave Management System

## Overview
The Leave Management System is a web-based application designed to manage employee leave applications efficiently. It tracks employee leave balances, processes leave requests, and ensures compliance with company policies. The system is built using PHP and MySQL.

## Features
- **Employee Management**: Manage employee details, including department, position, and contact information.
- **Leave Management**: Apply for, approve, or reject leave applications.
- **Leave Balance Tracking**: Track annual leave balances, ensuring employees do not exceed their allocated leave.
- **Financial Year Handling**: The system manages leave balances across financial years and allows the carry forward of unused leave days.

## System Requirements
- **Web Server**: Apache or any compatible web server.
- **PHP**: Version 7.4 or higher.
- **MySQL**: Version 5.7 or higher.
- **Browser**: Latest versions of Chrome, Firefox, or Edge.

## Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/pharlexj/leave-management-system.git
   ```
2. **Navigate to the project directory**:
   ```bash
   cd leave-management-system
   ```
3. **Configure the database**:
   - Import the `mydb.sql` file provided in the `/database` folder into your MySQL server.
   - Update the `config.php` file with your database credentials:
     ```php
     $servername = "your_servername";
     $username = "your_username";
     $password = "your_password";
     $dbname = "your_database_name";
     ```

4. **Start the web server**:
   - Ensure Apache and MySQL services are running.
   - Access the application via your web browser at `http://localhost/leave-management-system`.

## Usage

### Admin Login
- **Username**: `Admin`
- **Password**: `Admin`

### Employee Login
- Employees can log in using their email and password credentials provided by the HR department.

### Applying for Leave
1. Navigate to the "Apply for Leave" section.
2. Fill in the required details, including the start date, end date, and reason for leave.
3. Submit the application. The system will check the leave balance and notify the employee of any issues.

### Approving or Rejecting Leave (Admin)
1. Log in as an admin.
2. Go to the "Manage Leave Applications" section.
3. Review pending leave applications and either approve or reject them.

## Security
- Change the default admin username and password after the first login for security purposes.
- Ensure your `config.php` file is not exposed to the public.

## Troubleshooting
- **Database Connection Issues**: Double-check your `config.php` settings to ensure they match your database credentials.
- **Session Issues**: Ensure the `session_start()` function is called at the beginning of every script that requires session management.

## Contributing
If you want to contribute to this project, please fork the repository, create a new branch, and submit a pull request. Your contributions are welcome!

## License
This project is licensed under the MIT License. See the `LICENSE` file for more details.

---

This `README.md` should provide a clear overview of your project and guide users through installation, setup, and usage. Adjust the contents as necessary to reflect any additional features or specific instructions relevant to your system.
