# Automated-Blood-Donor-Mobilization-System
Automated Blood Donor Mobilization System
Project Overview
This is an n8n-based automation workflow designed to bridge the gap between blood requirements and eligible donors. It eliminates manual searching by instantly identifying and contacting donors via WhatsApp based on real-time requests.

Key Features
Instant Trigger: Activated via a website Webhook whenever a specific blood group is required.

Intelligent Filtering: Automatically scans a Google Sheets database and filters donors based on:

Matching Blood Group.

Eligibility (Only contacts donors who haven't donated in the last 5 months).

Automated Outreach: Sends personalized recruitment messages using the WhatsApp Business Cloud API.

Audit Trail: Automatically logs all contacted donors back into a "Sent History" sheet for tracking.

Tech Stack
Automation: n8n

Database: Google Sheets

Communication: WhatsApp Business API (Meta)

Trigger: Webhook (JSON POST)

How to Use
Import the blood-donor-automation.json file into your n8n instance.

Configure your credentials for Google Sheets and Meta (WhatsApp).

Set the Webhook URL in your website's "Submit" button logic.
