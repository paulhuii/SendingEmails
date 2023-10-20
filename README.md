# Mass Email Sender in Python

## Description

This Python script enables you to send mass emails using the Simple Mail Transfer Protocol (SMTP). The script reads the names and email addresses of recipients from a CSV file and sends them a personalized email.

## Prerequisites

- Python 3.x
- A CSV file named `names_emails.csv` containing the recipients' names and email addresses
- Access to an SMTP server

## Dependencies

- `smtplib` for sending emails via SMTP
- `csv` for reading CSV files

## How to Run

1. Place your `names_emails.csv` in the same directory as the script.
2. Run the script using `python your_script_name.py`.
3. Input your email address and password when prompted.

## CSV File Format

- The first column should contain the name of the recipient.
- The second column should contain the recipient's email address.
- I have included the CSV file in this repo for you to use.
- Make sure you write over the first row, there should be no headers.

Example:

```
John Doe,johndoe@example.com
Jane Doe,janedoe@example.com
```

## Code Overview

1. Import the necessary modules.
2. Read names and email addresses from the `names_emails.csv` file.
3. Initialize the SMTP server and login.
4. Send emails to all recipients in the CSV file.
5. Close the SMTP connection.

## Troubleshooting

- If authentication fails, an `SMTPAuthenticationError` will be raised.
- If the connection to the SMTP server cannot be established, an `SMTPConnectError` will be raised.
- For other issues, a general exception will be printed.

## Note

Make sure to modify the SMTP server and port according to your email provider's specifications.

## Customization

- Modify the `smtp_server` and `smtp_port` variables as per your requirements.
- The email subject and body can be modified in the `subject` and `body` variables.

## Author

Paul Hui, some google, and some ChatGPT
