Power Automate Staff Account Registration
This project automates the registration of new staff accounts using Power Automate in Microsoft 365.

Overview
When a new user submits the New Staff Information Sheet form, the automation will:

Check if the user’s personal email already exists in the form data.

If the personal email does not exist, it will:

Create a new organization email account.

Assign the Exchange Online (Plan 2) for students license.

Send a confirmation email to the user’s personal email containing their new organization email.

If the personal email exists, it will:

Stop the process.

Send an email to notify the user that they are already registered.

Email Format Rules
Organization email is generated using the first letter of the user’s first name + full last name.

Example: For user John Max, the email will be jmax@siraj.institute.

If a user with the same first and last name exists but with a different personal email, a number is appended.

Example: For the second John Max, the email will be jmax2@siraj.institute.

Features
Automated detection of duplicate registrations.

Automatic email creation with naming conflict handling.

License assignment for new accounts.

Notification emails for both new registrations and duplicate attempts.

Screenshots
(Add your screenshots here to illustrate key steps in the flow)

Technologies Used
Power Automate (Microsoft 365)

Microsoft Exchange Online

Microsoft Forms (New Staff Information Sheet)

How to Use
Submit the New Staff Information Sheet form with required user details.

Power Automate flow triggers automatically.

Check your email for confirmation or notification of existing registration.
