---
title: Privacy Policy | TimeBack
description: TimeBack Privacy Policy
lang: en
last_updated: 2026-06-06
---

# Privacy Policy (TimeBack)

- **App name:** TimeBack
- **Developer:** frog-im
- **Contact:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- **Effective date:** 2026-06-03
- **Last updated:** 2026-06-06

This Privacy Policy is based on the current implementation of the TimeBack app. TimeBack provides screen-time review, daily goals, reclaimed-time records, reflections, challenges, notifications, sharing, and advertising features.

## 1. Features

TimeBack provides the following features:

- App usage-time review through Android usage access permission
- Daily usage goals, reminders, and status-bar usage notifications
- Hard-limit warning notifications and overlay display
- Overlay exception app selection
- Reclaimed-time activity records
- Daily reflection records
- Challenge progress and checklist management
- Usage-stat image sharing
- Google AdMob ads and UMP-based privacy options

## 2. Information We Process

### 2-1. Information Read Through Usage Access Permission

If the user grants Android `PACKAGE_USAGE_STATS` permission, the app may read the following information from the device:

- App package name
- App name
- App usage time
- Date and time range used for usage aggregation

This information is used to provide usage statistics and compare usage against user goals.

### 2-2. Information Entered or Configured by the User

- Daily usage goal
- Usage reminder enabled state and interval
- Status-bar usage display setting
- Reclaimed-time activity category, title, start time, and duration
- Daily reflection text
- Challenge progress and checklist entries
- Overlay exception app list

### 2-3. Information Stored on the Device

The app may store the following information in a local SQLite database or SharedPreferences:

- App usage-time records
- Daily goals and settings
- Reclaimed-time activity records
- Daily reflection records
- Challenge progress and checklist state
- Onboarding completion state
- Settings such as usage reminders, hard-limit warnings, status-bar display, and overlay exception apps
- Local ad consent and privacy-option state

Based on the current implementation, these local records are not automatically uploaded to frog-im servers.

### 2-4. Advertising and Consent Data

When Google Mobile Ads SDK (AdMob) and UMP are used, Google or its affiliates may process information such as:

- Advertising identifiers, such as Android AD_ID
- IP address and network information
- Device information, OS version, and app information
- Ad impressions, clicks, measurement data, and error signals
- Ad consent and privacy-option state
- Approximate location

## 3. Purposes of Processing

The app processes information for the following purposes:

- Reading usage time, showing statistics, and comparing usage against goals
- Storing reclaimed-time and reflection records entered by the user
- Managing challenge progress
- Providing reminders and status-bar notifications
- Providing hard-limit warning notifications, overlay display, and overlay exception handling
- Sharing usage-stat images when requested by the user
- Serving ads, measuring ad performance, and applying ad consent choices
- Maintaining app stability and responding to errors

## 4. Local Storage and External Processing

### 4-1. Local Storage

TimeBack stores user data primarily in the app's internal storage on the device. Based on the current implementation, usage records, goals, reflections, and challenge information are not automatically uploaded to frog-im servers.

Local storage may include the following.

| Storage | Stored items | Purpose | Deletion method |
|---|---|---|---|
| SQLite database | App usage records, package names, app names, usage time, date-based aggregates | Show usage statistics and compare usage against goals | In-app deletion features, clearing app data, or uninstalling the app |
| SQLite database | Reclaimed-time activities, reflections, challenge progress, checklist entries | Show records and manage progress | In-app deletion features, clearing app data, or uninstalling the app |
| SharedPreferences | Onboarding completion state, reminder settings, hard-limit warning settings, status-bar display settings, overlay exception app list, local ad-consent state | Keep app settings | Clearing app data or uninstalling the app |
| Temporary files/cache | Shared usage-stat images and similar temporary files | Perform sharing requested by the user | Deleted after sharing where possible, or according to OS/app cleanup policies |

When the user clears app data or uninstalls the app, data stored in the app's internal storage is generally deleted. However, Android backup, manufacturer backup, cloud backup, or files directly shared by the user may be retained separately according to the policies of those services.

Usage records and reflection text may reveal personal routines or interests. On shared devices, users should use appropriate safeguards such as device lock or separate OS accounts.

### 4-2. Server Uploads

Based on the current project, TimeBack does not automatically upload usage records, reflections, or challenge records to frog-im servers. If the user uses the sharing feature, a generated statistics image may be transferred to the external app or service selected by the user.

### 4-3. Advertising Processing

Google AdMob and UMP are used for in-app advertising and consent management. Advertising-related information may be processed on Google infrastructure.

## 5. Third-party Services and Processors

### 5-1. Google AdMob / UMP

Purpose:

- Banner ad delivery
- Ad consent and privacy-option handling
- Ad performance measurement and fraud prevention

Information that may be processed:

- Advertising identifiers
- Device and network information
- Ad interaction information
- Consent and privacy-option state

### 5-2. Sharing Target Apps or Services

If the user directly uses the usage-stat image sharing feature, the selected external app or service may process the shared image. That processing is governed by the privacy policy of the selected service.

## 6. Cross-Border Transfer Notice

Information may be processed outside the user's country in the following cases.

| Item | Details |
|---|---|
| Recipient | Google LLC and its affiliates |
| Destination | United States and other countries/regions where Google infrastructure is located |
| Timing | When the app runs, requests ads, shows or measures ads, processes clicks, or handles consent |
| Method | Encrypted network communication (HTTPS/TLS) |
| Purpose | Ad delivery, personalization state handling, measurement, analytics, service stability improvement, legal compliance |
| Data | Advertising identifiers, device/app/network information, ad interaction information, consent state, approximate location, etc. |
| Retention | In accordance with Google's policies and applicable law |

For details, please see the [Cross-Border Transfer Notice](./policy/).

## 7. Installed App List and Overlay Exceptions

On Android, if the user configures overlay exception apps, the app may read the package names and app names of launchable apps on the device to display a selection list. Package names selected by the user as exceptions are stored in SharedPreferences on the device and are used only to avoid showing hard-limit warning overlays on top of those apps.

## 8. Retention

The app retains information under the following standards:

- Local usage, goal, reflection, and challenge information: until the user deletes it, clears app data, or uninstalls the app
- SharedPreferences settings: until the user clears app data or uninstalls the app
- Temporary files for shared images: as needed for sharing or according to OS cleanup policies
- Advertising and consent-related data: according to the policies of Google and other relevant third parties

## 9. Permissions

The app may use the following permissions:

- `PACKAGE_USAGE_STATS`: read app usage time
- `POST_NOTIFICATIONS`: show usage reminders and status-bar notifications
- `SYSTEM_ALERT_WINDOW`: show hard-limit warning overlays
- `INTERNET`: communicate with ad SDKs and show legal notice pages
- `ACCESS_NETWORK_STATE`: check network state
- `com.google.android.gms.permission.AD_ID`: use advertising identifiers

Permissions are used only as needed for app features. Users may revoke permissions in device settings, but related features may be limited.

## 10. User Rights and Choices

Users may:

- View, edit, or delete records inside the app
- Delete local information by clearing app data or uninstalling the app
- Change usage access, notification, and advertising identifier settings in device settings
- Revoke overlay permission and change overlay exception app settings
- Change ad privacy options
- Contact us with privacy questions or deletion requests

Contact email: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

## 11. Security Measures

The app applies or may apply the following safeguards:

- HTTPS/TLS-based external communication
- Local-first data processing
- Minimum permission requests needed for app features
- Application of advertising consent state

Device security conditions such as rooting, jailbreaking, malware, or shared-device use may create additional risks.

## 12. Children's Privacy

TimeBack is not designed primarily for children. Age-related settings or platform policies of Google Mobile Ads SDK and UMP may apply during advertising and consent processing.

## 13. Changes

This Policy may be updated due to changes in law, third-party service configuration, or app features. Material changes will be notified through in-app notice or by updating this page.

## 14. Contact

- Developer: frog-im
- Email: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
