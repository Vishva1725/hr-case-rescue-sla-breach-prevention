# Implementation Guide

## Project
HR Case Rescue – SLA Breach Prevention

## Objective
Monitor Payroll HR cases against their resolution SLA and provide visibility into SLA progress through ServiceNow notifications.

## Technologies
- ServiceNow HR Service Delivery (HRSD)
- SLA Definitions and Task SLA
- Flow Designer
- Scoped Applications
- Update Sets
- Email Notifications

## SLA Configuration
- SLA name: HR Case Rescue - Payroll Resolution
- Target table: HR Payroll Case
- Duration: 30 minutes
- Schedule: 24 x 7
- HR service: Payroll Query Resolution

## Automation
The project includes a Flow Designer flow named `HR Case Rescue - SLA Warning` for monitoring eligible Task SLA records and attempting to send warning emails.

## Validation
- Created a test Payroll HR case.
- Verified that a Task SLA was attached.
- Observed SLA elapsed time and remaining time.
- Received SLA progress notification emails in Gmail.
- Captured screenshots of the configuration and test results.

## Deployment Notes
1. Review the Update Set XML for sensitive information.
2. Import the Update Set into an authorized target ServiceNow instance.
3. Preview the Update Set and resolve any conflicts or errors.
4. Commit the Update Set.
5. Validate the SLA definition, flow, and notification behavior in the target instance.

## Limitations
Validate the custom warning flow's email action independently before using it in production. Some earlier outbound email records were ignored by the email subsystem.

## Disclaimer
This is a personal learning project built and tested in a ServiceNow Personal Developer Instance (PDI). It is not a production deployment.
