# DSNC Food Online Order Platform — Turkshop & Restaurant

Welcome to the DSNC Food Online Order project! This repository provides the codebase and resources for an online food ordering system developed for the Directory Zambia Nation Science Centre (DSNC), specifically focused on Turkshop and Restaurant services.

## Overview

The DSNC Food Online Order Platform enables customers to conveniently browse menus, place food orders, and make payments online. The system is designed to streamline the ordering process for both the Turkshop and DSNC Restaurant, providing a seamless digital experience for users.

# Science Centre

A robust, modular web application platform for online food ordering, restaurant, and shop management. Built with **PHP** and **CodeIgniter**, it supports extensible modules, secure installation, and customizable features, making it ideal for scalable deployments.

---

## Features

- **Built on CodeIgniter:** Fast, lightweight PHP framework.
- **Modular Architecture:** Easily extend functionality by installing or updating modules and addons.
- **Online Ordering:** Manage food orders and restaurant/shop operations.
- **Secure Installation:** Guided installer with environment checks.
- **User Authentication:** Login and access control for administrators and users.
- **Database Integration:** Automated database migrations for new modules.
- **Theming Support:** Customizable UI themes.
- **RESTful APIs:** Integrate with external services and SDKs.
- **Multi-language Support:** Easily localize your platform.

---

## Installation

### Prerequisites

- PHP 7.2 or higher
- MySQL/MariaDB database
- Apache/Nginx web server
- Composer (for dependency management)
- Git (recommended)

### Steps

1. **Clone the Repository**
   ```bash
   git clone https://github.com/brightonmasumba/science-centre.git
   cd science-centre
   ```

2. **Install Dependencies**
   - For PHP dependencies (with Composer):
     ```bash
     composer install
     ```
   - For Node.js dependencies (if applicable):
     ```bash
     npm install
     ```

3. **Configuration**
   - Set up your database and update configuration files in `application/config/`.
   - Set proper file permissions for `application/modules/`, `assets/`, and `install/`.

4. **Run the Installer**
   - Access `http://your-domain/install` in your browser.
   - Follow on-screen instructions to complete setup.
   - On completion, delete the `install` folder from your server's root directory as instructed for security.

5. **Launch the Application**
   - Access `http://your-domain/login` to begin using the platform.

---

## Usage

1. **Login:** Use admin credentials created during installation.
2. **Manage Modules/Addons:** Navigate to the dashboard to install, update, or remove modules.
3. **Order Management:** Access restaurant/shop modules to handle orders and customer management.
4. **Customization:** Change themes, configure settings, and install external SDKs as needed.

---

## Contribution Guidelines

We welcome contributions from the community! To contribute:

1. **Fork the Repository**
2. **Create a Feature Branch**
   ```bash
   git checkout -b feature/your-feature-name
   ```
3. **Commit Your Changes**
   ```bash
   git commit -m "Add your feature"
   ```
4. **Push and Open a Pull Request**
   ```bash
   git push origin feature/your-feature-name
   ```
   - Submit a pull request describing your changes.

**Guidelines:**
- Follow [CodeIgniter](https://codeigniter.com/user_guide/general/styleguide.html) and PSR standards for PHP code.
- Document new modules/features thoroughly.
- Ensure your code passes all CI checks.
- See [CONTRIBUTING.md](CONTRIBUTING.md) for details.

---

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## Support

For issues, bug reports, or feature requests, please open an issue in this repository.

---
## Contact

For questions, suggestions, or collaboration opportunities, open an issue or contact the maintainer at [brightonmasumba](https://github.com/brightonmasumba).
