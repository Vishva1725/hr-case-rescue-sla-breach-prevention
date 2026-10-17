# HR Case Rescue – SLA Breach Prevention

## Overview
A ServiceNow HR Service Delivery (HRSD) project that monitors Payroll HR cases and demonstrates SLA progress tracking and notification workflows.

## Problem Statement
HR cases can miss their resolution targets when approaching deadlines are not identified early enough. This project explores SLA monitoring and notification mechanisms to help HR teams identify cases that need attention.

## Technologies
- ServiceNow HR Service Delivery (HRSD)
- SLA Definitions and Task SLAs
- Flow Designer
- Scoped Applications
- ServiceNow Update Sets
- Email Notifications

## Key Features
- Custom 30-minute Payroll Resolution SLA
- SLA tracking for eligible Payroll HR cases
- SLA progress notifications
- Flow Designer-based warning automation
- Configuration export using a ServiceNow Update Set

## Implementation
1. Create the scoped application.
2. Configure the Payroll Query Resolution HR service.
3. Create the custom Payroll Resolution SLA definition.
4. Configure the SLA warning flow.
5. Create test HR cases and verify Task SLA records.
6. Validate notification delivery and package configuration changes.

## Testing Status
The custom SLA was attached to test HR cases, and SLA progress notification emails were received.

The custom Flow Designer warning email action still requires validation because some generated email records were marked as ignored.

## Deployment
Review the exported Update Set and its dependencies before importing it into an authorized ServiceNow instance. Preview the Update Set, resolve any errors or collisions, and verify the application after committing.

## Screenshots
See the `screenshots/` folder for implementation evidence.

## Disclaimer
This is a learning and portfolio project. Review all exported configuration for credentials, keys, personal data, and sensitive information before sharing publicly.
