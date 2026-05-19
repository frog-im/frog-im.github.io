---
title: Privacy Policy | QDiary
description: QDiary Privacy Policy
---

# Privacy Policy (QDiary)

- App Name: QDiary
- Developer: frog-im
- Contact: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- Effective Date: 2026-04-19
- Last Updated: 2026-04-19

This Privacy Policy is written based on the current implementation of the QDiary app. QDiary provides diary writing, quest generation and reflection, login, manual cloud save, advertising, and notification features, and in that process may process personal information or information that may constitute personal information to the extent necessary.

## 1. Features Provided

QDiary provides the following features:

- Writing, editing, and viewing diaries
- Category classification and calendar view
- Quest generation, quest reflection, and quest completion handling
- Local diary app lock and local encryption
- Email login, email verification, anonymous (guest) login, and password reset
- User-initiated cloud save and load
- Ad display and ad privacy options handling
- Quest reminder notifications

## 2. Categories of Information Processed

### 2-1. Information Entered Directly by the User

- Email address
- Password
- Diary title, body, date, category, and difficulty
- Quest responses, reflection content, and selected quest information
- Quest profile-related selections and summary text
- Passphrase for diary app lock

### 2-2. Information Stored by the App on the Device

- Local diary DB (SQLite)
- Quest status information for local diaries
- Attendance, settings, language, notifications, and ad-related state values
- App lock verification values, salt, and encryption metadata
- Quest notification scheduling information

### 2-3. Account and Identification Information

The following information may be processed through Firebase Authentication:

- Firebase UID
- Email address
- Whether email verification has been completed
- Whether anonymous login is being used

### 2-4. Advertising and Consent Information

When using Google AdMob and the UMP SDK, the following information may be processed:

- Advertising identifiers (such as Android AD_ID)
- IP address and network information
- Device information, OS version, and app information
- Ad impressions, clicks, and reward processing information
- Ad consent status and privacy option status

### 2-5. Notification-Related Information

- Whether notification permission has been granted
- Identifier values for diaries that contain ongoing quests
- Quest notification text
- Scheduled notification times

## 3. Purposes of Processing

The app processes information for the following purposes:

- Sign-up, login, email verification, and password reset
- Writing, saving, and viewing diaries
- Quest generation, reflection, and completion determination
- Local encryption and decryption associated with app lock
- Cloud save and load requested by the user
- Providing quest notifications
- Providing ads, processing ad rewards, and reflecting ad consent status
- Security, error handling, and service operation

## 4. Local Storage, Cloud Storage, and External Processing

### 4-1. Local Storage

Diary and quest information is primarily stored in the device’s local DB.

- If app lock is not enabled: stored locally in general form
- If app lock is enabled: some information, such as diary title, body, and quest status, may be encrypted and stored locally

### 4-2. Cloud Storage

The app stores data in Firebase Firestore only when the user directly executes the `Save` feature.

Under the current project configuration:

- Automatic full synchronization is not used
- Data is stored in Firestore `savedDiaries` only when the user manually saves it
- When saved, the diary title, body, and quest status may be stored in encrypted form depending on the current app lock status
- Data is loaded back to local storage only when the user executes `Load`

### 4-3. External Processing for Quest Generation and Reflection

When the user requests quest generation or reflection, the following information may be used for external processing through Firebase Functions:

- Diary title
- Diary body or reflection body
- Category
- Difficulty
- Selected quest
- Quest profile summary information

This information is used for quest generation and evaluation through the OpenAI API.

Important:

- Related diary content is used for external processing only when the quest feature is used.
- Under the current project configuration, code that stores quest logs in a separate `questLogs` collection is not used.

## 5. Third-Party Services and Outsourced Processing

### 5-1. Google Firebase

Purpose:

- Authentication (Firebase Authentication)
- Firestore storage
- Cloud Functions execution

Information that may be processed:

- UID, email address, and authentication status
- Diary data manually saved by the user
- Quest request data

### 5-2. OpenAI

Purpose:

- Quest generation
- Quest reflection and completion evaluation

Information that may be processed:

- Diary title/body
- Quest text
- Difficulty and category
- Reflection content entered by the user
- Quest profile summary information

### 5-3. Google AdMob / UMP

Purpose:

- Providing banner, interstitial, and rewarded ads
- Handling ad consent and privacy options

Information that may be processed:

- Advertising identifiers
- Device and network information
- Ad interaction information
- Consent status

## 6. International Transfer Notice

The app may process personal information or related information outside the user’s country in the following cases:

| Item | Details |
|---|---|
| Recipient | Google LLC, OpenAI, and related infrastructure operators |
| Destination Country | United States, etc. |
| Timing of Transfer | During login, quest generation/reflection, ad requests, and consent processing |
| Method of Transfer | Encrypted network communication |
| Purpose of Transfer | Authentication, data storage, serverless processing, AI quest generation/evaluation, and advertising |

## 7. Retention and Use Period

The app retains information according to the following standards:

- Local diary/settings information: until the user deletes it or uninstalls the app
- Firebase account information: while the user maintains the account
- Firestore stored data: while the user keeps the saved items
- Quest request processing data: to the extent necessary for serverless processing
- Ad/consent-related data: according to each external provider’s policy

In addition, the current project includes the following automatic cleanup logic:

- Cleanup of anonymous user accounts and user subcollection Firestore data after a certain period
- Cleanup of long-inactive regular user accounts and user subcollection Firestore data

However, whether this is actually reflected in the production environment may vary depending on deployment status and server settings.

## 8. App Lock and Local Encryption Notice

The app provides a separate `Diary App Lock` feature.

- The app lock passphrase is separate from the account password.
- The app lock passphrase is used for local diary encryption and decryption.
- Even if an incorrect passphrase is entered, the app itself may not always be completely blocked; instead, some diary content may remain unreadable.
- Some diaries may be encrypted separately based on the passphrase used at the time of writing or temporary unlock.

Users should keep their passphrase safe, and if it is lost, recovery of some local data may be difficult.

## 9. Quest Notification Notice

If the user enables quest notifications, local notifications may be scheduled for each diary with an ongoing quest.

- Scheduling is mainly handled through internal device scheduling.
- Under the current project configuration, there is no confirmed structure in which diary source text is periodically transmitted to a central server solely for notification purposes.

## 10. Permission Usage Notice

The app may use the following permissions to provide its features:

- `INTERNET`: communication with Firebase, OpenAI, and ad SDKs
- `com.google.android.gms.permission.AD_ID`: use of advertising identifiers
- `POST_NOTIFICATIONS`: displaying quest notifications
- `RECEIVE_BOOT_COMPLETED`: restoring scheduled notifications after device reboot

Permissions are used only to the extent necessary to perform the relevant functions.

## 11. Rights of the Data Subject and How to Exercise Them

Users may exercise the following rights:

- Access, modify, and delete data within the app
- Delete or overwrite cloud-stored data
- Request logout and account deletion
- Change ad privacy options
- Disable notification permissions

How to exercise these rights:

- Directly delete or edit diaries within the app
- Delete the app or reset local data
- Log out of the account and separately request deletion
- Change notifications, advertising identifiers, and permissions in device settings
- Contact email: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

## 12. Security Measures

The app applies or may apply the following protective measures:

- HTTPS-based communication
- Local diary app lock and encryption
- Separate storage of passphrase verification values
- Use of Firebase Authentication
- Minimum permission requests

However, risks may arise depending on the user’s device security status, such as rooting, jailbreaking, malware, or use of a shared device.

## 13. Children’s Personal Information

The app is not designed as a service primarily intended for children. However, age-related options within UMP may be applied during ad/consent processing.

## 14. Changes to This Policy

This Policy may be revised due to changes in laws, third-party services, or app features.

- Last updated for the current version: **2026-04-19**

## 15. Contact

- Developer: frog-im
- Email: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- Account deletion guide: [Deletion instructions](https://docs.google.com/forms/d/e/1FAIpQLSexIrSPRwSmVG5aU-Mp0wq0uRyXTh2Xh9Gag3Y4QBisWmFZWw/viewform?usp=dialog)

