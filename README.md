# Property Management System

A Django-based property management platform designed to manage properties, units, tenants, leases, rent, payments, maintenance, expenses, documents, and reports from a centralized system.

> 🚧 **Project Status:** In development

## Overview

The **Property Management System (PMS)** is being built as a production-style Django project and as a foundation for learning backend development with Django and PostgreSQL.

The project focuses on real-world property-management workflows instead of a basic CRUD implementation, including role-based access, relational data, financial tracking, maintenance workflows, document management, dashboards, and reporting.

## Planned Modules

### Authentication & User Management

- Admin
- Property Manager
- Owner
- Tenant
- Login and logout
- Role-based permissions
- User profiles

### Properties

- Property management
- Buildings
- Units
- Property details
- Occupancy status
- Property photos
- Property documents

### Tenants

- Tenant profiles
- Tenant history
- Lease information
- Tenant documents
- Rental history

### Lease Management

- Lease creation and management
- Start and end dates
- Monthly rent
- Security deposits
- Payment due dates
- Lease status
- Lease documents

### Rent & Payments

- Rent tracking
- Due dates
- Payment records
- Outstanding rent
- Partial payments
- Overdue payments
- Payment methods
- Receipts

### Maintenance

- Maintenance requests
- Request categories
- Priority levels
- Assignment tracking
- Request status
- Maintenance history
- Resolution tracking

### Expenses

- Property expenses
- Expense categories
- Vendor records
- Invoice/document uploads
- Expense history

### Dashboard & Reports

- Property overview
- Unit occupancy
- Tenant overview
- Rent collection
- Outstanding payments
- Expenses
- Maintenance statistics
- Financial summaries
- Property performance reports

## User Roles

| Role | Main Access |
|---|---|
| **Admin** | Full system access and administration |
| **Property Manager** | Properties, tenants, leases, rent, maintenance, expenses, and reports |
| **Owner** | Own properties, financial information, and reports |
| **Tenant** | Own profile, lease, payments, documents, and maintenance requests |

## Technology Stack

- **Backend:** Django
- **Frontend:** HTML, CSS, JavaScript
- **Database:** PostgreSQL
- **Version Control:** Git & GitHub

React is intentionally not part of the initial stack. The first version uses Django Templates to build a strong understanding of Django's request/response lifecycle, templates, forms, authentication, ORM, permissions, and server-rendered applications.

## Django Concepts Covered

This project is intended to provide hands-on experience with:

- Django project and app structure
- Models and model relationships
- Django ORM
- QuerySets and database queries
- Views
- URL routing
- Templates
- Template inheritance
- Forms and validation
- Authentication
- Authorization and permissions
- Django Admin
- Sessions
- File and image uploads
- Static and media files
- Dashboard aggregation and business logic
- PostgreSQL integration
- Testing
- Deployment

## Project Structure

```text
Property-Management-System/
│
├── manage.py
├── config/
│   ├── settings.py
│   ├── urls.py
│   ├── asgi.py
│   └── wsgi.py
│
├── apps/
│   ├── accounts/
│   ├── properties/
│   ├── tenants/
│   ├── leases/
│   ├── rent/
│   ├── maintenance/
│   ├── expenses/
│   ├── documents/
│   └── reports/
│
├── templates/
├── static/
├── media/
├── requirements.txt
└── README.md
```

> The project structure will evolve as development progresses.

## Development Roadmap

```text
Phase 1  → Django Fundamentals
Phase 2  → Authentication & User Roles
Phase 3  → Properties & Units
Phase 4  → Tenants & Leases
Phase 5  → Rent & Payments
Phase 6  → Maintenance
Phase 7  → Expenses
Phase 8  → Documents
Phase 9  → Dashboard
Phase 10 → Reports
Phase 11 → Permissions & Security
Phase 12 → Testing
Phase 13 → Deployment
```

## Getting Started

### Prerequisites

Make sure the following are installed:

- Python 3.x
- pip
- PostgreSQL
- Git

### Clone the repository

```bash
git clone https://github.com/Saksham1105/Property-Management-System.git
cd Property-Management-System
```

### Create and activate a virtual environment

#### Windows

```bash
python -m venv venv
venv\Scripts\activate
```

#### macOS / Linux

```bash
python3 -m venv venv
source venv/bin/activate
```

### Install dependencies

```bash
pip install -r requirements.txt
```

### Configure environment variables

Create a `.env` file for local configuration and database credentials.

Example:

```env
SECRET_KEY=your-secret-key
DEBUG=True
DB_NAME=property_management
DB_USER=postgres
DB_PASSWORD=your-password
DB_HOST=localhost
DB_PORT=5432
```

Do not commit real secrets or production credentials to GitHub.

### Run migrations

```bash
python manage.py makemigrations
python manage.py migrate
```

### Create a superuser

```bash
python manage.py createsuperuser
```

### Start the development server

```bash
python manage.py runserver
```

Then open the local development server in your browser.

## Database

PostgreSQL is the target database for the project. SQLite may be used temporarily during early experimentation, but the application is being designed around PostgreSQL for the full implementation.

## Security

The project will follow Django security practices including:

- Password hashing through Django authentication
- CSRF protection
- Permission checks on server-side views
- Secure handling of uploaded files
- Environment-based secrets
- Separation of development and production settings

## Learning Philosophy

This project is being developed as a hands-on Django foundation project.

The goal is not simply to produce a working application, but to understand how each major part of a production web application works:

```text
Requirement
   ↓
Database Design
   ↓
Django Models
   ↓
ORM Queries
   ↓
Views
   ↓
Forms
   ↓
Templates
   ↓
Authentication & Permissions
   ↓
Business Logic
   ↓
Testing
   ↓
Deployment
```

## Future Expansion

After the Django foundation is complete, the system can be extended with APIs and eventually integrated with a separate modern frontend or other services.

Potential future additions include:

- Django REST Framework APIs
- Notifications
- Email integration
- Online payment integration
- Advanced analytics
- Mobile application support
- AI/ML-assisted property analytics

## License

This project is distributed under the license included in the repository.

## Author

**Saksham1105**

GitHub: [@Saksham1105](https://github.com/Saksham1105)
