# Google App Scripts, Twilio, and WhatsApp Integration for Email Notifications

## Project Overview
This project enables automatic SMS notifications via WhatsApp for unread emails using Google App Scripts, Twilio, and an external Node.js server. When a user has unread emails, an SMS is sent to a specified number—typically the email owner—to alert them about their unread messages.

## Features
- **Email Monitoring**: Automatically checks for unread emails in a user's Gmail account.
- **SMS Notifications**: Sends notification messages through WhatsApp using Twilio's messaging API.
- **Customizable Alerts**: Users can set which email labels to monitor and define notification intervals.

## Prerequisites
- A Google Cloud Platform account with access to Google App Scripts.
- A Twilio account with WhatsApp messaging capabilities.
- Node.js installed on your local machine or server.
- Basic understanding of JavaScript and Node.js for server setup.

## Getting Started

### Setting up the Google App Script
1. Open Google Apps Script and create a new project.
2. Paste the provided Google Apps Script code into the script editor.
3. Save and name your project.
4. Set the Google App Script triggers to run at your preferred interval (e.g., every 5 minutes).

### Configuring Your Twilio Account
1. Sign up or log in to your Twilio account.
2. Set up WhatsApp sandbox following the instructions provided in your Twilio dashboard.
3. Obtain your Account SID and Auth Token from the Twilio Console.

### Setting Up the Node.js Server
1. Clone the repository to your local machine or server.
2. Install necessary dependencies by running:
`npm install`
3. Create an `.env` file in the root directory and add the following environment variables:
4. Start the server using:
`node server.js`


## How It Works
- **Google App Script**: Monitors the Gmail account for unread emails based on specific labels.
- **Node.js Server**: Receives data from Google App Script and utilizes the Twilio API to send SMS notifications via WhatsApp.
- **Twilio API**: Manages the delivery of SMS messages to the user's WhatsApp number.

## Usage
To receive notifications, ensure that your Gmail account, Node.js server, and Twilio WhatsApp messaging are properly configured. Notifications will be sent automatically according to the triggers set in Google App Scripts.

## Contributing
Feel free to fork this project and contribute by submitting a pull request. We appreciate improvements to the codebase, especially in enhancing the robustness of the email checking and SMS sending functionalities.
