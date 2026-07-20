# importHolidaysIntoEasyAppointments

A small web-based utility to import holiday data into the [Easy!Appointments](https://easyappointments.org/) scheduling system.

> ⚠️ **Notice**: This project is in active development!

## Overview

This project provides a simple frontend and backend to load holiday definitions and import them into your installed version of Easy!Appointments as blocked periods.

## Features

- Easy import of holiday entries into Easy!Appointments
- Select preferred country, subdivison, language, date range
- Choose explicity which holidays should be imported into your instance of Easy!Appointments
- Web browser interface via `index.html`
- No third-party services or server involved

## Usage

Use the hosted interface directly at [https://cn-tools.github.io/importHolidaysIntoEasyAppointments/](https://cn-tools.github.io/importHolidaysIntoEasyAppointments/) hosted by Github Pages.

## CORS

When using the hosted interface from GitHub Pages, CORS (Cross-Origin Resource Sharing) issues may occur when trying to communicate with your Easy!Appointments installation. To resolve this:

- Ensure your Easy!Appointments server is accessible and properly configured to accept requests from the GitHub Pages domain
- Consider running the application locally instead (clone the repository and open `index.html` locally)
- Alternatively, deploy this tool on the same domain as your Easy!Appointments installation to avoid CORS restrictions

---

## Development

### Requirements

- Easy!Appointments installation (local or online)
- Optional: Web server environment such as XAMPP, Apache or Nginx

### Installation

1. Clone or copy this repository into a local folder.
2. If not active yet, activate API access in your preferred instance of Easy!Appointments.
3. Go to "Try" ;)

### Try

1. Open `src/index.html` in your browser.
2. Use the interface to select or define holiday entries.
3. Submit the data to import holidays into Easy!Appointments.
4. Verify the inserted holidays in the Easy!Appointments admin calendar.

### Notes

- Adjust file permissions if necessary to allow the application to read and write data.
- Review Easy!Appointments configuration to ensure the holiday data is accepted correctly.

---

## License

This project is licensed under the MIT License.
