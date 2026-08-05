# importHolidaysIntoEasyAppointments

A small web-based utility to import holiday data into the [Easy!Appointments](https://easyappointments.org/) scheduling system.

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

> **⚠️ Since Easy!Appointments v1.6.0**, a stricter CORS check is active.\
Please therefore check the options listed below.

## CORS

When using the hosted interface from GitHub Pages, CORS (Cross-Origin Resource Sharing) issues may occur when trying to communicate with your Easy!Appointments installation. To resolve this:

#### Option 1 (recommended)

 To avoid CORS restrictions, install this tool on the same domain as your Easy!Appointments installation. To do this, download the latest [version](https://github.com/cn-tools/importHolidaysIntoEasyAppointments/releases) and upload the `index.html` file from folder `src` to the same domain as your Easy!Appointments installation. If necessary, rename the `index.html` file to prevent overwriting an existing one. Then, open your preferred browser, go to the corresponding page, and follow the instructions in the wizard.

#### Option 2

To use the application directly from GitHub Pages, your Easy!Appointments instance must allow cross-origin requests from `https://cn-tools.github.io`

Configure `CORS_ALLOWED_ORIGINS` accordingly and ensure that CORS preflight requests (`OPTIONS`) are handled correctly. The server must allow at least the following:

- Origin: `https://cn-tools.github.io`
- Headers: `Authorization`, `Content-Type`
- Methods: `GET`, `POST`, `PUT`, `PATCH`, `DELETE`, `OPTIONS`

Example response headers:

```http
Access-Control-Allow-Origin: https://cn-tools.github.io
Access-Control-Allow-Headers: Authorization, Content-Type
Access-Control-Allow-Methods: GET, POST, PUT, PATCH, DELETE, OPTIONS
```

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
