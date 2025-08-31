
# Apex Identity

**Apex Identity** is a secure authentication and user identity management solution designed for Oracle APEX applications.
It provides features such as encrypted login, role-based access control, and audit logging, making it easy to integrate enterprise-level security into APEX projects.

---

## Features

* 🔒 **Secure Login** – Supports encrypted password transmission to prevent credential theft.
* 🛡 **Role-Based Access Control** – Easily assign roles and permissions to users.
* 📜 **Audit Logging** – Track login attempts, failures, and session activities.
* 🗄 **Database-First Security** – All security rules stored and managed in Oracle Database.
* 🌐 **Multi-Branch Access** – Supports multi-branch or multi-tenant authentication logic.
* 🛠 **Easy Integration** – Designed to work seamlessly with existing Oracle APEX applications.

---

## Prerequisites

Before installing **Apex Identity**, make sure you have:

* **Oracle Database** 19c or later
* **Oracle APEX** 22.1 or later
* **SQL Developer** or another Oracle-compatible IDE
* Access to an **APEX workspace** with administrator privileges

---

## Installation

1. **Clone or Download** the project:

   ```bash
   git clone https://github.com/yourusername/apex-identity.git
   ```

2. **Import the Application** into your Oracle APEX workspace:

   * Log in to your APEX workspace.
   * Navigate to **App Builder → Import**.
   * Select the application export **ZIP file** (`.zip`) from this repository.
   * Follow the wizard to complete the installation.

3. **Database Objects** are created automatically during the import process:

   * All required tables, packages, and supporting objects will be installed.
   * No additional schema setup is required.

4. Once imported, run the application directly from your workspace and configure initial users and roles.

---

## Database Tables

The following tables are included in **Apex Identity**:

* **T\_USERS** – Stores system user accounts, including login credentials and profile details.
* **T\_ROLES** – Defines available roles in the system (e.g., Admin, Manager, User).
* **T\_USER\_ROLES** – Links users to one or more roles.
* **T\_ROLE\_PERMISSIONS** – Defines which pages, menus, buttons, and regions are accessible by each role.
* **T\_USER\_ACTIVITY\_LOG** – Tracks user login attempts, activity history, and audit logs.
* **T\_BRANCHES** – Stores branch/organizational unit information, used for multi-branch access control.

---
Application Overview

You can manage user roles directly within the application:

Create new roles or edit existing ones in the User Roles page.

By clicking on a role name, you can assign the required permissions.

The system automatically loads all pages, menus, buttons, and regions of the application, allowing you to easily grant the necessary access to each role.

## Authorization for Items

Any item that should follow the rules of this authorization must have its Authorization property set to Dynamic Authorization.

## License

This project is licensed under the **MIT License** – you are free to use, modify, and distribute it with proper attribution.

  ## Contact
For questions, support, or feedback, please reach out via email: s.jabbari77[@]gmail[.]com
