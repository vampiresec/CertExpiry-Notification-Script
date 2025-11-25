# CertExpiry Notification Script
A PowerShell-based automation solution that monitors self signed and the SP certificate expiration dates in PingFederate connections and proactively notifies application owners before certificates expire.
## Overview
This script leverages the PingFederate Admin API to automatically fetch connection and certificate expiry information, then sends timely email notifications to application owners at critical intervals to prevent service disruptions due to expired certificates.

## Features

- **Automated Certificate Monitoring**: Retrieves certificate expiration details from PingFederate connections via REST API
- **Multi-Stage Notifications**: Sends email alerts at configurable intervals:
  - 30 days before expiry
  - 15 days before expiry
  - 7 days before expiry
  - 2 days before expiry

- **Application Owner Targeting**: Delivers notifications directly to responsible application owners
- **PingFederate Integration**: Seamless integration with PingFederate Admin API for real-time certificate data

## Use Case
Ideal for IAM teams managing PingFederate federation environments who need to ensure certificate renewals are completed before expiration, preventing authentication failures and service outages.

## Requirements
- PowerShell 5.1 or later
- PingFederate Admin API access
- SMTP server configuration for email notifications

## Technologies
- PowerShell
- PingFederate Admin API
- SMTP/Email Services
