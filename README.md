application:
Property Management Ltd Application
Overview
The Property Management Ltd application is designed to streamline tenant management and booking requests. It features three primary tables:

Tenants - Stores all relevant tenant information.
Management Booking - A form that allows tenants to submit service requests, such as maintenance issues or inspections.
Property Listings - Contains details about property addresses and their availability.

Booking Form Functionality
The Management Booking form includes several fields:

Tenant Details: Information about the tenant.
Urgency: A dropdown to indicate the priority level (1, 2, or 3).
Type of Service: Options for maintenance or inspection.
If maintenance is selected, a dependent field appears allowing tenants to specify the type of service needed (e.g., structure, plumbing, appliance, or other).
If inspection is selected, a field for date and time becomes available.
UI Policies and Actions are used to dynamically show or hide fields based on tenant selections. Notifications are set up to alert employees or managers of pending tasks.

Email Handling
To protect tenant information, two email fields are included in the form. When a tenant submits their email, a flow checks it against the tenant details table. If there’s a match, it populates the tenant's information (full name, address, phone number) while safeguarding against unauthorized access to data from other tenants.

Table Structures

Tenant Details Table: Contains full names, addresses, emails, and phone numbers.
Property Address Table: Stores available properties and their addresses.
Service Catalog Integration
To ensure tenants can easily access the booking form, I've created catalog items and a record producer:

Maintenance Record Producer: This includes fields for the email mentioned above, type of service, service details (conditional based on maintenance or inspection), and a description field for tenant issues.
Handyman Insurance: An optional service with three pricing options (premium, standard, basic) that tenants can select.
Rental Property Submission: Allows prospective tenants to request rental properties. The form includes fields for property selection, monthly income confirmation (over $4000), full name, first name, phone number, and email. Approved applicants become tenants and can submit maintenance requests.
Dashboard and Reporting:
A dashboard is generated for managers monthly, displaying:

Number of bookings
Property availability
Types of services requested
Number of tenants
Reports are consolidated into a single dashboard for easy viewing.
Knowledge Article:
A tenancy agreement article is accessible in the knowledge section for tenant reference.

Flow Implementation:
Five key flows have been established to automate processes:

Handyman Insurance Booking: Checks if the requester is a tenant and processes the request accordingly.
Maintenance Task Assignment: Assigns tasks based on urgency and type, with inspections routed to managers.
Inspection Reminder: Sends an email reminder six months after an inspection request.
New Tenant Onboarding: Validates tenant income and property availability, updating records as necessary.
Address Parsing: Uses advanced business rules to separate full addresses into street, postcode, country code, and city for better data management.
Future Development
