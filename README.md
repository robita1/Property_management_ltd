Property Management Ltd Application

Overview

The Property Management Ltd Application is designed to streamline tenant management and booking requests. It includes features for tenant data storage, property listings, and service request management.

Key Features
1. Tenant Management
Tenants Table: Stores all relevant tenant information (e.g., full names, addresses, emails, and phone numbers).
Email Handling: Protects tenant information using validation.
A flow checks the submitted email against the tenant details table.
Populates tenant information (full name, address, phone number) securely.
2. Booking Requests
Management Booking Form Table:
Includes fields for:
Tenant Details: Basic tenant information.
Urgency: Priority dropdown (Levels 1, 2, or 3).
Type of Service: Options for maintenance or inspection.
If Maintenance: Dependent fields for service type (e.g., structure, plumbing, appliance, other).
If Inspection: Fields for scheduling date and time appear dynamically.
UI Policies and Actions: Dynamically show or hide fields based on tenant selections.
Notifications: Alerts employees or managers about pending tasks.
3. Property Listings
Property Address Table:
Stores property addresses and their availability.

Service Catalog:
Maintenance Record Producer: Fields for tenant email, service type, conditional service details, and descriptions of tenant issues.
Handyman Insurance: An optional service with three pricing options (Premium, Standard, Basic).
Rental Property Submission: Fields for property selection, monthly income confirmation (over $4000), full name, phone number, and email.
Approved applicants are converted into tenants who can submit maintenance requests.

Automation and Workflows: Handyman Insurance:
Verifies tenant status before processing requests.
Update Fields for maintenance Task Assignment:
Routes tasks based on urgency and service type, with inspections assigned to managers.
Inspection Reminder:
Sends email reminders six months after an inspection request.
New Tenant Onboarding:
Validates income and property availability, updating records as necessary.
Look up Tenant details: To populate tenant details

Business rules: for separating full addresses into street, postcode, country code, and city for improved data management.

Dashboard and Reporting:
A consolidated manager dashboard displays:
Number of bookings.
Property availability.
Types of services requested.
Number of tenants.
Reports are generated monthly for strategic insights.

Knowledge Management:
Tenancy Agreement for tenant.


