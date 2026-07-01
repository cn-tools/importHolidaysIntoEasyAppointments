# importHolidaysIntoEasyAppointments

A small web-based utility to import holiday data into the EasyAppointments scheduling system.

## Overview

This project provides a simple frontend and backend to load holiday definitions and inject them into EasyAppointments.

## Features

- Easy import of holiday entries into EasyAppointments
- Web browser interface via `index.html`
- Simple installation for local or XAMPP deployments
- No third-party service or server involved

## Usage

Use the hosted interface directly at [https://cn-tools.github.io/importHolidaysIntoEasyAppointments/](https://cn-tools.github.io/importHolidaysIntoEasyAppointments/) hosted by Github Pages.

---

## Development

### Requirements

- PHP 7.4 or newer
- EasyAppointments installation
- Optional: Web server environment such as XAMPP, Apache, or Nginx

### Installation

1. Clone or copy this repository into your web server folder.
2. Place the files inside the EasyAppointments installation directory or into a subfolder that can access your EasyAppointments database and configuration.
3. Ensure that PHP is available and the web server can execute the script.

### Try

1. Open `index.html` in your browser.
2. Use the interface to select or define holiday entries.
3. Submit the data to import holidays into EasyAppointments.
4. Verify the inserted holidays in the EasyAppointments admin calendar.

### File Structure

- `index.html` - Web interface for importing holiday data.
- `README.md` - This documentation.

### Notes

- Adjust file permissions if necessary to allow the application to read and write data.
- Review EasyAppointments configuration to ensure the holiday data is accepted correctly.

---

## License

This project is licensed under the MIT License.
