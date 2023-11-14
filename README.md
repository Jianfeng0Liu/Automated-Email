# Automated-Email

## I. Introduction
This project aims to develop an interactive interface that automates the process of drafting and sending emails based on the current date. The interface should be user-friendly and capable of handling file uploads and custom inputs. The application will be developed using Python and Flask and will be deployed on Azure for easy access.

## II. Requirements
1. The interface should allow users to upload a file with a maximum size limit of 20MB per email.
2. The system should automatically fetch the current date and day of the week (in Japanese format), and incorporate this information into the email subject and body.
3. Users should have the option to input additional information, which should be inserted into the email body before the closing salutation. If no additional information is provided, this section should be omitted.
4. Upon clicking ‘Send’, the system should automatically send the email to a predefined list of recipients, with the option to CC other email addresses. The recipient and CC addresses should be editable and saved for future use.
5. The system should integrate with Microsoft Outlook, which the user is already logged into on their computer. The application should not require the user to input their account credentials.

## III. Realization
1. **Development Environment**: The application will be developed using Python and Flask. Python is chosen for its extensive libraries that simplify many complex tasks. Flask is a lightweight web framework perfect for this type of application.
2. **File Uploads**: File uploads will be handled using Flask’s request object. A maximum file size limit of 20MB will be set to ensure the uploaded files do not exceed the email size limit.
3. **Fetching Date and Day**: The datetime library in Python will be used to fetch the current date and day of the week. This information will be formatted appropriately and incorporated into the email subject and body.
4. **Email Creation and Sending**: The smtplib and email.mime libraries in Python will be used to create and send emails. These libraries provide all the necessary functionalities for email handling.
5. **Integration with Outlook**: The SMTP server of Outlook (smtp.office365.com) will be used to send emails. This allows the application to integrate seamlessly with the user’s existing Outlook account, which they are already logged into on their computer.
6. **Recipient and CC Addresses**: The recipient and CC addresses will be stored within the application. If the user edits these addresses, the application will update the stored addresses accordingly.
7. **Deployment on Azure**: Finally, the application will be deployed on Azure. This allows the user to access the application via a web browser without the need to install any software on their computer.
