# Gmail-Push
A mail pusher for gmail, through ssl.

"""
# Email Sending Script

## Overview

This Python script demonstrates how to send an email using Gmail via the SMTP_SSL protocol. It utilizes the `smtplib` library and the `EmailMessage` class from the `email.message` module.

## Usage

### Prerequisites

1. Python installed on your system.
2. Gmail account with the necessary permissions.
3. Enable "Less secure app access" on your Gmail account settings.

### Instructions

1. Replace the placeholder values in the script with your own email and password.

    ```python
    email_sender = 'your_email@gmail.com'
    email_password = 'your_app_password'
    email_reciever = 'recipient_email@example.com'
    ```

    - `email_sender`: Your Gmail email address.
    - `email_password`: Your Gmail app password. [Generate one here](https://myaccount.google.com/apppasswords).
    - `email_reciever`: Email address of the recipient.

2. Update the subject and body of the email as needed.

    ```python
    subject = "Work Schedule Change"
    body = "Work starts one hour late from tomorrow"
    ```

3. Run the script.

    ```bash
    python email_script.py
    ```

### Security Considerations

- **App Passwords:** For improved security, generate and use an [App Password](https://myaccount.google.com/apppasswords) instead of your regular Gmail password. This ensures that your main password is not exposed in the script.

- **Environment Variables:** Consider using environment variables to store sensitive information like email and password. Modify the script accordingly to read values from environment variables.

    ```python
    import os

    email_sender = os.environ.get('EMAIL_SENDER')
    email_password = os.environ.get('EMAIL_PASSWORD')
    email_reciever = os.environ.get('EMAIL_RECEIVER')
    ```

    Set the environment variables before running the script.

## Disclaimer

This script is provided as-is and may be subject to changes based on updates to the libraries or security considerations. Use it responsibly and in accordance with Gmail's terms of service.
"""
