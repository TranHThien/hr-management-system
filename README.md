# Human Resource Management System (HRM)

A comprehensive Human Resource Management system built with **ASP.NET MVC**, designed to streamline organizational processes including employee management, payroll, and contracts.

## Overview

The HRM System provides a centralized platform for HR professionals and administrators to manage their workforce efficiently. It features a modern user interface powered by **Tailwind CSS** and a robust backend integrated with **SQL Server**.

## Key Features

### Employee Management
- Full lifecycle management of employees (Add, View, Update, Disable).
- Detailed profiles including personal information, contact details, and job status.
- Department mapping and organizational hierarchy.

### Contract Management
- Manage different contract types (Probation, Full-time, Seasonal).
- Configure basic salary and salary coefficients.
- Tracking of contract validity and expiry dates.

### Payroll & Timekeeping
- **Timekeeping:** Track daily attendance for all employees.
- **Monthly Payroll:** Automatic calculation of salaries based on base pay, coefficients, and attendance.
- **Payment Status:** Monitor and update payment status for monthly salary tables.

### Department Management
- Create and manage organization departments (e.g., HR, Accounting, IT).
- Assign employees to specific departments.

### Reports & Statistics
- Analytical dashboards for HR oversight.
- Statistical data on workforce distribution and payroll expenses.

### Role-Based Access Control (RBAC)
- **Admin:** System configuration and high-level management.
- **Human Resources (HR):** Operational management of employees, contracts, and payroll.
- **Employee:** Personal information access and employee self-service.

## Technology Stack

- **Backend:** ASP.NET MVC (.NET Framework 4.7.2), C#
- **Database:** Microsoft SQL Server
- **Frontend:** HTML5, CSS3, JavaScript
- **Styling:** Tailwind CSS, Font Awesome, Google Fonts (Inter)
- **Design:** StarUML (Logic/Class/ERD Modeling)

## Project Structure

- `human_resource_management/`: Main web application project.
  - `Areas/Admin/`: Admin dashboard and system settings.
  - `Areas/HumanResource/`: Core HR operations (Employees, Payroll, Stats).
  - `Areas/Employee/`: Employee portal.
  - `Controllers/`: Application logic.
  - `Views/`: Application UI templates.
  - `Models/`: Data entities and logic.
- `_db.sql`: Primary database schema script.
- `Nhom_2_Lan_1.mdj`: StarUML design file.

## Installation & Setup

1. **Database Setup:**
   - Open SQL Server Management Studio (SSMS).
   - Execute the `_db.sql` script to create the `QuanLyNhanSu` database and its tables.

2. **Project Setup:**
   - Open the solution file `human_resource_management.sln` in **Visual Studio**.
   - Update the connection string in `Web.config` to match your local SQL Server instance.
   - Restore NuGet packages (right-click Solution > Restore NuGet Packages).

3. **Run:**
   - Press `F5` or click **Start** in Visual Studio to run the application on IIS Express.

## License

This project is developed for academic purposes as part of the NTU Semester 1 (2025-2026) curriculum.
