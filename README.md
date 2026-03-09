# Client Onboarding Automation (Make.com)

## Overview

This project demonstrates an automated client onboarding workflow built with **Make.com**.
The system captures form submissions, creates CRM contacts, sends onboarding emails, schedules meetings, and notifies the team automatically.

The goal is to reduce manual administrative work and ensure that every new lead receives immediate follow-up.

---

## Workflow

1. A user submits a **Google Form**.
2. The automation scenario is triggered in **Make.com**.
3. A new contact is created or updated in **HubSpot CRM**.
4. The system checks the selected **plan type**.
5. Based on the plan, the workflow follows different paths:

   * sends a personalized onboarding email
   * schedules a meeting in Google Calendar
   * notifies the manager in Slack.

---

## Automation Logic

### Premium Plan

* Sends a **Premium welcome email**
* Schedules a meeting **within 1 day**
* Sends a Slack notification about the new Premium client

### Basic Plan

* Sends a **Basic welcome email**
* Schedules a meeting **within 3 days**
* Sends a Slack notification about the new Basic client

---

## Tech Stack

* **Make.com** – workflow automation platform
* **Google Forms** – lead capture
* **HubSpot CRM** – contact management
* **Gmail** – automated email communication
* **Google Calendar** – meeting scheduling
* **Slack** – internal team notifications

---

## Architecture

Google Forms
→ HubSpot CRM (Create or Update Contact)
→ Router (Plan-based branching)

**Premium branch**
→ Gmail (Send Email)
→ Google Calendar (Create Event)
→ Slack (Send Notification)

**Basic branch**
→ Gmail (Send Email)
→ Google Calendar (Create Event)
→ Slack (Send Notification)

---

## Business Value

* Eliminates manual lead processing
* Ensures immediate response to new clients
* Standardizes the onboarding process
* Reduces risk of missed leads
* Improves internal team awareness

---

## Example Use Cases

This workflow can be used for:

* course registrations
* consulting onboarding
* SaaS client intake
* agency lead management
* service booking systems

---

## Future Improvements

* advanced error handling
* automated follow-up sequences
* lead scoring
* CRM pipeline automation
* webhook integrations

---

## Author

Automation workflow built using **Make.com** to demonstrate CRM-driven onboarding automation.
