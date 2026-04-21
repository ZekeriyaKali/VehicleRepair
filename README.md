# Vehicle Repair MVC

Vehicle Repair MVC is a web-based application developed with ASP.NET Core MVC that manages vehicle service processes end-to-end. The system enables users to create appointments, track repair processes, and generate invoices, while administrators manage operations through a dedicated admin panel.

---

## Project Overview

This project is designed to digitalize vehicle service management workflows. It provides a structured system where users and administrators interact through clearly separated roles and responsibilities.

The application includes appointment management, repair tracking, notification handling, and invoice generation features.

---

## Technologies Used

* ASP.NET Core MVC
* Entity Framework Core
* Microsoft SQL Server
* Session-based Authentication
* iText7 (PDF generation)

---

## Features

### User Features

* User registration and login
* Vehicle registration
* Appointment creation
* Viewing appointment status
* Appointment cancellation with time constraints
* Notification tracking
* Invoice viewing and PDF download

### Admin Features

* Dashboard for monitoring users and vehicles
* Appointment approval and rejection
* Repair process management
* Product and stock management
* Notification creation for users

---

## Application Workflow

1. Users register and log in to the system
2. Users add their vehicles
3. Users create service appointments
4. Administrators review and approve or reject appointments
5. Approved appointments proceed to repair processes
6. Notifications are sent to users
7. Users can view and download invoices

---

## Project Structure

```
VehicleRepairMVC/
├── Areas/
│   └── Admin/
│       ├── Controllers/
│       │   ├── AppointmentController.cs
│       │   ├── DashboardController.cs
│       │   ├── ProductController.cs
│       │   └── RepairProcessController.cs
│
├── Controllers/
│   ├── HomeController.cs
│   ├── AppointmentController.cs
│   ├── LoginController.cs
│   ├── NotificationController.cs
│   └── ProfileController.cs
│
├── Models/
│   ├── User.cs
│   ├── Car.cs
│   ├── Appointment.cs
│   ├── RepairProcess.cs
│   ├── Product.cs
│   └── Notification.cs
│
├── Context/
│   └── VehicleRepairDbContext.cs
│
└── Program.cs
```

---

## Authentication

The system uses session-based authentication to manage user login states. Separate access flows are implemented for standard users and administrators.

---

## Invoice Generation

Invoices are dynamically generated using iText7. Each invoice includes detailed repair processes and total cost calculations. Users can download invoices in PDF format.

---

## Setup Instructions

Clone the repository:

```
git clone <repository-url>
cd VehicleRepairMVC
```

Update the database connection in `appsettings.json`:

```

Run the project:

```
dotnet restore
dotnet run
```

---

## Notes

This project demonstrates practical implementation of MVC architecture, database management, and workflow-driven application design. It is suitable for showcasing backend and full-stack development skills in professional environments.
