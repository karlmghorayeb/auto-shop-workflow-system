# Collision Shop Workflow Management System

> **Note:** To protect the privacy of the business and its customers, all sensitive information shown in this repository has been blurred or replaced with sample data. The source code is not public because this was developed for a real business.

---

## Overview

This system was built for an automotive collision repair shop to improve their daily workflow. Before the system was created, employees relied on physical folders for each vehicle, handwritten updates, and communication through walkie-talkies to keep track of repair progress. When customers wanted updates about their vehicles, employees often had to manually search for the latest information.

I built a web application that centralized repair tracking, parts management, and customer communication into one place. The application was built with Flask, uses Google Sheets as a backend database, and integrates with the Twilio API to automatically send text message updates to customers.

---

## Skills

- Python
- Flask
- HTML
- CSS
- Google Sheets API
- Twilio API
- Git
- Railway

---

# Walkthrough

## Employee Login

![Login Page](screenshots/Login%20Page.png)

Employees access the application through a secure PIN-protected login page.

---

## Home Page

![Home Page](screenshots/Home%20Page.png)

The home page allows employees to quickly navigate between the Vehicle Tracker, Parts Tracker, and Text Dashboard.

---

## Vehicle Tracker

![Car Tracker Page](screenshots/Car%20Tracker%20Page.png)

The Vehicle Tracker is the main part of the application. Employees can:

- View all active repairs
- Search for vehicles
- Add new repairs
- Edit customer and vehicle information
- Update repair statuses
- Assign technicians, painters, and detailers
- Delete repair orders


---

## Parts Tracker

![Parts Tracker Page](screenshots/Parts%20Tracker%20Page.png)

The Parts Tracker helps employees keep track of incoming parts by allowing them to:

- Add ordered parts
- Automatically fill customer information and vendor names for efficiency
- Search for vehicles
- Keep notes for each part

---

## Automated Customer Text Messages

![Text Dashboard](screenshots/Text%20Dashboard%20Page.png)

The system automatically sends personalized customer updates through the Twilio API whenever a vehicle reaches certain repair stages.

Examples include:

- Waiting for Parts
- In Repair
- In Paint
- Detailing
- Ready for Pickup

This allowed customers to stay updated without needing to call the business for progress updates.

---

## Example Customer Texts

<img src="screenshots/Example%20Text%20Messages.png" width="350">

Examples of automated messages sent to customers during the repair process.

---

## Customer Review Portal
![Review Portal Page](screenshots/Review%20Portal%20Page.png)

After a customer picks up their vehicle, the system automatically sends a text message containing a link to the shop's review portal, which directs customers to different review websites.

---

## Google Sheets Integration
Google Sheets acts as the backend database for all information. Changes made on the website reflect on the sheet and vice versa.

### Car Tracker Database

![Car Tracker Sheet](screenshots/Car%20Tracker%20Sheet.png)

Stores active repair status, customer information, and timestamps regarding SMS Messages.

---

### Car Tracker Archive

![Car Tracker Archive Sheet](screenshots/Car%20Tracker%20Archive%20Sheet.png)

Completed repairs are moved into an archive sheet to preserve records of past repairs.
---

### Parts Database

![Part Tracker Sheet](screenshots/Part%20Tracker%20Sheet.png)

Stores received parts, vendors, and notes associated with each vehicle.

---
