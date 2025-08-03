New Staff Account Automation with Power Automate 🚀
This project demonstrates an automated workflow for managing new staff account creation and registration using Microsoft Power Automate within a Microsoft 365 environment. The automation streamlines the onboarding process, ensuring efficiency and accuracy while handling common exceptions like duplicate entries and name conflicts.

🌟 Project Overview
The core of this project is a Power Automate flow that triggers when a new user submits the "New Staff Information Sheet" form. The flow automates several key steps, including:

Duplicate Entry Detection: Checks if the user's personal email is already in the system.

Unique Account Creation: Generates a new, standardized organizational email address.

License Assignment: Assigns the appropriate license to the new user account.

User Notification: Sends a confirmation email with the new account details or a rejection email if the user is already registered.

Username Conflict Resolution: Handles cases where a new user has a name similar to an existing user by adding a numerical suffix to the new username.

💡 Key Features
Seamless Integration: Integrates directly with Microsoft Forms, Outlook, and Microsoft 365 user management.

Error Handling: Prevents duplicate account creation and notifies users accordingly.

Intelligent Logic: Automatically handles username conflicts to ensure unique email addresses (e.g., jmax@siraj.institute vs. jmax2@siraj.institute).

Automated Communication: Reduces manual effort by sending automated confirmation or rejection emails.

Security: Assigns a specific license, "Exchange Online (Plan 2) for students", ensuring correct access permissions from the start.

⚙️ Workflow Logic
The Power Automate flow follows this logical sequence:

Trigger: A user submits a new entry to the "New Staff Information Sheet" form.

Lookup: The flow searches the existing user data to see if the submitted personal email address already exists.

Conditional Check:

IF the personal email is found: The flow sends a "registration already exists" email and stops.

IF the personal email is not found: The flow proceeds.

Username Generation:

It generates a new email based on the format: first letter of first name + last name + @siraj.institute.

It then checks if this newly generated email is already in use by another user.

IF the email is already in use (username conflict): It appends a number to the last name (e.g., jmax2@siraj.institute) and re-checks for uniqueness until a non-conflicting email is generated.

Account Creation: The flow creates a new user account in Microsoft 365 with the unique email address.

License Assignment: The "Exchange Online (Plan 2) for students" license is assigned to the new user.

Final Notification: A confirmation email is sent to the user's personal email, providing them with their new organizational email and instructions.

🖼️ Screenshots
🛠️ How to Adapt This Project
This project can be easily adapted to different organizations by modifying a few key parameters:

Email Domain: Change @siraj.institute to your organization's domain.

License Type: Adjust the license assigned to new users based on organizational needs.

Form Source: The trigger can be modified to use other data sources like a SharePoint list or an Excel spreadsheet.

Email Content: The content of the confirmation and rejection emails can be customized.

🤝 Contribution
Feel free to fork this repository and adapt the workflow to your own needs. If you have suggestions or improvements, please submit a pull request!
