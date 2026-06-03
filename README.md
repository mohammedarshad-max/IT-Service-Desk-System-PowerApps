# IT Service Desk System

## Overview

The IT Service Desk System is a business application developed using Microsoft Power Apps, Dataverse, and Power Automate. The solution streamlines the process of raising, tracking, assigning, and resolving IT support tickets within an organization.

Employees can submit IT support requests, monitor ticket progress, and receive automated notifications, while IT administrators can manage, assign, and close tickets through a centralized dashboard.

---

## Business Problem

Organizations often rely on emails or manual processes to manage IT support requests, resulting in delayed responses, poor visibility, and inefficient tracking.

This solution provides a centralized platform to:

* Submit IT support requests
* Track ticket progress
* Assign tickets to support personnel
* Manage ticket lifecycle
* Automate notifications and updates

---

## Key Features

### Employee Features

* Raise IT support tickets
* Provide issue details and category
* Track ticket status
* View ticket history
* Receive automated email notifications
* View ticket submission confirmation

### IT Support Features

* View all submitted tickets
* Assign tickets to technicians
* Update ticket status
* Add resolution notes
* Close completed tickets
* Monitor support workload

### Automation Features

* Automatic email notification when a ticket is created
* Automatic email notification when a ticket is closed
* Status-based workflow automation using Power Automate

---

## Technology Stack

| Technology                  | Purpose             |
| --------------------------- | ------------------- |
| Microsoft Power Apps        | User Interface      |
| Microsoft Dataverse         | Data Storage        |
| Microsoft Power Automate    | Workflow Automation |
| Microsoft Outlook Connector | Email Notifications |
| Power Fx                    | Application Logic   |

---

## Solution Architecture

Employee
↓
Power Apps
↓
Dataverse
↓
Power Automate
↓
Email Notifications

IT Team
↓
Dashboard
↓
Ticket Assignment
↓
Status Updates
↓
Ticket Resolution

---

## Application Screens

### Home Dashboard

Provides an overview of the system and quick navigation options.

Features:

* Welcome Banner
* Navigation Buttons
* Ticket Metrics

---

### Raise Ticket Screen

Allows users to submit support requests.

Fields:

* Requester Name
* Requester Email
* Category
* Priority
* Description

---

### Success Screen

Displayed after successful ticket submission.

Features:

* Confirmation Message
* Ticket Submission Acknowledgement
* Navigation Options

---

### My Tickets Screen

Displays all tickets submitted by the user.

Features:

* Ticket List
* Status Tracking
* Ticket Details Access

---

### Ticket Details Screen

Displays complete information for a selected ticket.

Features:

* Ticket Information
* Assigned Technician
* Resolution Notes
* Current Status

---

### IT Dashboard

Used by support personnel for ticket management.

Features:

* View All Tickets
* Assign Tickets
* Monitor Ticket Status
* Update Resolution Information

---

## Dataverse Tables

### Tickets

| Column Name      | Data Type       |
| ---------------- | --------------- |
| Ticket Number    | Auto Number     |
| Requester Name   | Text            |
| Requester Email  | Text            |
| Category         | Choice          |
| Priority         | Choice          |
| Description      | Multi-line Text |
| Status           | Choice          |
| Assigned To      | Text            |
| Resolution Notes | Multi-line Text |
| Created On       | Date & Time     |

---

## Power Automate Flows

### Flow 1: Ticket Creation Notification

Trigger:

* When a new ticket is created

Actions:

* Send email notification
* Acknowledge ticket submission

---

### Flow 2: Ticket Closure Notification

Trigger:

* When ticket status changes to Closed

Actions:

* Send closure email to requester
* Confirm successful ticket resolution

---

## Benefits

* Centralized ticket management
* Improved visibility of support requests
* Faster response times
* Automated communication
* Improved operational efficiency
* Better user experience

---

## Future Enhancements

* Role-Based Access Control
* SLA Monitoring
* Escalation Management
* Technician Workload Dashboard
* Microsoft Teams Notifications
* AI-Powered Ticket Categorization
* Reporting and Analytics


## Author

Mohammed Arshad A

AI Engineer | Power Platform Developer

Skills:

* Microsoft Power Apps
* Microsoft Power Automate
* Dataverse
* Power Platform Solutions
* Workflow Automation
* Business Process Automation

---

## Project Status

Completed and available for demonstration and further enhancements.
