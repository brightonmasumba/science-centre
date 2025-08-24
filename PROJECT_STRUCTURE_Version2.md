# Project Structure and Main Components

This documentation explains the key folders, files, and main classes of the Science Centre project, built with PHP and CodeIgniter.

---

## Top-Level Structure

### Root Directory

- **index.php**  
  The front controller for CodeIgniter. All requests are routed through this file, which bootstraps the framework and loads the correct controller.

- **README.md**  
  Contains project overview, installation, usage, and contribution information.

---

## Application Folder

The `application/` directory contains all your application-specific code.

- **config/**  
  Configuration files, including database, autoload, and routing.

- **controllers/**  
  Main controllers for routing requests. Example: `Installer.php` handles installation logic.

- **modules/**  
  Custom modules implementing the modular architecture:
  - **dashboard/**  
    Core admin and user dashboard logic.
    - `controllers/Module.php`, `controllers/Autoupdate.php` — Handle module management and auto-update features.
  - **addon/**  
    Handles add-on/module installation, verification, and management.
    - `controllers/Module.php` — Class with methods for module CRUD, install/uninstall logic, verification, and database migration.
  - **template/**  
    UI templates and sidebar/menu management.
    - `views/includes/sidebar.php` — Contains sidebar menu definition and PHP logic for navigation.

- **views/**  
  All HTML and PHP template files for rendering output.  
  Contains installer views (for setup wizard), themes, and plugin documentation.

---

## System Folder

The `system/` directory contains the CodeIgniter core framework files.

- **helpers/**  
  Helper functions for various operations.
  - `directory_helper.php` — Contains the `directory_map` function for recursively mapping folder contents.
- **libraries/**  
  Core libraries, e.g., `Zip.php` for handling ZIP file creation and extraction.

---

## Themes and Plugins

- **application/views/themes/**  
  Contains different UI themes, assets, and third-party plugin integrations.
  - **defaults/** and **classic/** — Theme folders.
    - `assets_web/plugins/` — Plugin directories (e.g., `owl-carousel`, `lightslider-master`), each with its own README and documentation.

---

## JavaScript and Assets

- **assets/**  
  Static assets like CSS, JS, images.

- **application/modules/accounts/assets/js/treeview_script.js**  
  Provides UI logic for treeview menus in accounts or sidebar.

---

## Main Classes and Their Roles

- **Module.php (dashboard/addon/controllers)**  
  - Handles module installation, update, verification, deletion
  - Manages module database migrations, file extraction, permissions, and CRUD

- **Installer.php (controllers)**  
  - Manages the installation wizard, environment checks, and cleanup after install

- **Autoupdate.php (dashboard/controllers)**  
  - Handles automated updates, temporary file management, and update verification

---

## Sidebar/Menu Definition

- **sidebar.php (template/views/includes)**
  - Defines the navigation structure for the admin dashboard
  - Uses PHP arrays for controller/method/permission mapping
  - Supports sections like Kitchen management, Accounting, Addons, Themes, Roles and Permissions

---

## Example Code Snippet: Directory Helper

```php
function directory_map($source_dir, $directory_depth = 0, $hidden = FALSE)
{
    // Recursively reads the directory and builds an array representation
}
```
*Usage: Used for listing modules, assets, etc.*

---

## Plugin and Theme Documentation

- Plugins like Owl Carousel and LightSlider include their own documentation and contribution guides within their folders.
- Themes provide customizable UI layouts and assets.

---

## Contribution to Modular Architecture

- Each module has its own controllers, models, views, and assets.
- Modules can be installed, updated, or removed independently, with database migrations handled automatically.

---

## Summary

This structure enables scalable, modular development using CodeIgniter conventions, allowing easy extension through modules and add-ons, centralized asset and theme management, and secure installation and updates.

For details on each module/class, refer to the inline PHPDoc comments and module README files.
