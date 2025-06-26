# Google Workspace Backup tool for effective backup and recovery

This repository provides guides for using [Google Workspace Backup](https://www.nucleustechnologies.com/google-workspace-backup/)

Backup Gmail, contacts, calendar/appointments, Google Groups, and Google Drive data from Google Workspace to local drive &amp; NAS

## Features

- Flexible Backup Formats: Export data in multiple formats including PST, MSG, EML, PDF, DOC, DOCX, MHT, or HTML.
- Comprehensive Backup: Backup Google Contacts, Google Drive, Shared Drive, Google Groups, Gmail, and Calendar seamlessly.
- Incremental Backup: Perform incremental backups to avoid duplication, transferring only newly added data.
- Offers advanced Filter options, such as Date Filter, Item Type Filter, and more for selective data backup.
- Bulk Backup: Back up multiple Google Workspace user mailboxes using batch CSV imports for large-scale data protection. 
- Import PST to Google Workspace account with Kernel Google Workspace Backup and Restore (formerly G Suite backup).
- Restore PST to Google Groups of the selected Google Workspace mailbox.
- No need for Outlook installation on the system to restore PST files.


## Why Should You Back Up Google Workspace Emails?

While Google Workspace offers a retention period for deleted items, its native tools do not support recovery of accidentally or permanently deleted data. To prevent critical data loss, it is recommended to use a third-party backup tool. Here are the primary risks that highlight the need for a Google Workspace backup solution:

### Accidental Deletion or Data Overwriting

In environments where multiple users collaborate on a project, accidental file deletions or overwriting are common. If essential data is mistakenly deleted or overwritten, a reliable backup solution is necessary to restore the original content.

### Cyber Threats, Malware, or Ransomware Attacks

Cyber-attacks, malware infections, and ransomware are prevalent threats to organizations using Google Workspace. The cost of encryption recovery or dealing with ransomware attacks can be significant. Rather than spending heavily on recovery solutions, a proactive backup strategy ensures your data remains safe and recoverable.

### Unauthorized Access or Internal Threats

In cases of unauthorized access (e.g., account breaches) or insider threats (e.g., intentional data leakage by an employee), data confidentiality may be compromised. A backup ensures that sensitive information can be restored even if access is lost.

###  SaaS Outages and Technical Issues

SaaS outages and other technical issues may disrupt workflows, sometimes causing potential data loss during service interruptions. By relying on a backup tool, you can protect vital data and ensure uninterrupted access, even in case of an outage.

### Data Loss During Migration

When performing the data migration for a merger or acquisition of a business organization, the risk of data loss increases by 2X because of source and destination permissions. Creating a backup of old data is necessary for every organization to avoid data loss and fulfill legal compliances.

### Employee leaving the organization

When an employee leaves the organization, the respective user account needs to migrate their data into a safer place and perform deletion. However, before migration and deletion of the account, all the crucial data from Google Workspace must be backed up to the local or network drive of the system.

## Why Choose Kernel Google Workspace Backup and Restore Tool?

Unlike Google Workspace built-in recovery options, which can be limited and restrictive (especially after permanent deletion), third-party tools like Google Workspace Backup provide a robust, scalable solution to ensure data protection and compliance. 

![Meet Compliance Requirements](https://www.nucleustechnologies.com/imagenew20/feature-icons/g-suite-backup/meet-compliance-requirement.png)

### Meet Compliance Requirements

Ensure that your organization adheres to legal, regulatory, and industry compliance standards. With the ability to store data for specific periods, The tool facilitates data retention and supports compliance with various regulations.

![Zero downtime backup](https://www.nucleustechnologies.com/imagenew20/feature-icons/g-suite-backup/zero-downtime-backup.png)

### Zero downtime backup

Backup operations do not have to interfere with your ongoing business processes. It is designed for zero downtime, meaning you can back up your critical data without disrupting daily operations.

![Security Features](https://www.nucleustechnologies.com/imagenew20/feature-icons/g-suite-backup/security-features.png)

### Enhanced Security Features

We prioritize data security, ensuring that backups are accurate and complete. Data is protected using advanced encryption techniques. The Google Workspace backup tool connects to Google Workspace using secure credentials such as Service Account Email, Account Login ID, and P12 key.


## How to use

1. Download the Google workspace backup software (https://www.nucleustechnologies.com/downloads/kernel-g-suite-backup.exe)
2. Click on Backup tile and then click the +Add button to add the G Suite account for backup.
3. Configure service account (use P12 or JSON key)
4. Apply the required filters and click I am OK, Start Migration.
5. Select output type of backup
6. After backup save report to CSV


## Technical FAQs about Google Workspace backup tool

I cannot back up Contacts and Calendar/Appointments. What should I do?

To back up Contacts and Calendar/Appointments, ensure that the required Google API is enabled for your domain. To enable the API:

- Go to go to - https://console.developers.google.com.
- Go to your domain and ensure the new/existing project has the required API enabled.

I received an error "Google.Apis.Requests.Request Error User-rate limit exceeded." How can I resolve this?

This error occurs when the API request limit is exceeded. You need to increase the API quota by following these steps:

- Log in to the Google cloud platform using the URL [https://console.cloud.google.com](https://console.cloud.google.com/)
- In the IAM and admin category, click on **Quotas**.

- Choose the API whose limit you want to increase. Then, choose the **Edit Quotas** option.

- Input a new limit and click the **Submit Request** option.

Similarly, you can change the quota limit of other APIs too.

What is the difference between P12 and JSON keys?

P12 keys come with a certificate in the form of a PKCS#12 bundle, whereas JSON keys can obtain the certificate from Google SDK website. This is the primary distinction between P12 and JSON keys. A JSON Web Token (JWT) is signed with the certificate and sent to Google OAuth 2.0 servers to request an access token. After that, API requests are authorized using the access token.

## Sample CSV Format
```csv
Email, UserDisplayName
user1@yourdomain.com, User One
user2@yourdomain.com, User Two
user3@yourdomain.com, User Three
user4@yourdomain.com, User Four
