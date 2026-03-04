---
title: Privacy Policy | know_me
description: know_me (PeopleNote, Memory for People) Privacy Policy (English)
---

# Privacy Policy (know_me / PeopleNote, Memory for People)

- **App Name:** know_me (PeopleNote, Memory for People)
- **Developer:** frog-im
- **Personal Information Protection Officer / Contact Person:** frog-im
- **Contact:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- **Effective Date:** 2026-03-04
- **Last Updated:** 2026-03-04

> This Policy has been prepared based on the information processed by the app and its related features.  
> If any mandatory laws or regulations apply in a specific country or region, such laws or regulations may take precedence.

---

## 1. Purpose and Scope

`know_me` is an app designed to help users record and manage information about people, and, when needed, back up, restore, and share such information as PDF files.

Its main features include:

- Storing person-specific information (such as name, identifying text, notes, personality traits, country, gender, contact information, etc.)
- Folder classification, search, and merge functions
- Photo attachment and description management
- Exporting and importing backups (`.knm`)
- Exporting PDFs
- App lock (password/pattern)
- Advertising and consent management (AdMob/UMP)

The app does not require separate account registration, and the core user data of the app is generally stored locally on the user's device.  
However, certain third-party SDKs included for advertising and consent management may process some information.

---

## 2. Categories of Personal Information Processed

### 2-1) Information Entered Directly by the User

The following information is stored only when the user enters it directly:

- Name
- Identifying text (such as appearance/features used as memo text)
- Notes
- Personality traits, country, gender
- Phone number
- Text related to appearance time / time of meeting
- Platform/site information
- Folder name/color
- Image description (caption)

### 2-2) Files Selected on the Device

- Image files selected by the user when attaching photos
- `.knm` backup files selected by the user when importing backups
- Save paths and saved files selected by the user when exporting PDFs/backups

### 2-3) Data Stored Locally Within the App

The following data may be stored on the user's device in order to provide app features:

- SQLite DB (`people_note.db`): metadata for people/folders/platforms/sites/images
- Image files: encrypted and stored within the app documents folder (`.enc`)
- App settings (`SharedPreferences`): theme, sorting, privacy/ad options, PDF masking options, app lock policies, etc.
- App lock information: hash values and salts for passwords/patterns (`SharedPreferences`)
- Local encryption keys: stored in `flutter_secure_storage`
- Temporary files: image decryption previews, import/export cache files, etc. (temporary folder)

### 2-4) Information That May Be Processed Automatically During Advertising and Consent Handling

When advertising or consent management features are enabled, SDKs of Google LLC and related partners (such as AdMob and UMP) may automatically process the following information:

- Advertising identifiers (AAID/IDFA, etc.)
- IP address and network information
- Device information (OS version, device model, app version, etc.)
- Ad interaction information (impressions, clicks, etc.)
- Consent status and privacy choice information
- Diagnostic, performance, and security-related information

The app's core user records are not generally uploaded to the developer's server, but some of the above information may be transmitted to third-party services while advertising/consent features are in use.

---

## 3. Purpose of Processing Personal Information

The app processes personal information or related information for the following purposes:

- Recording and browsing people-related information centered on contacts/notes
- Providing organization features such as folder classification, search, and merge
- Attaching and displaying photos
- Performing user-requested functions such as backup/restore and PDF export
- Providing app lock security features
- Providing advertising, managing consent, preventing fraudulent activity, and complying with legal obligations

---

## 4. Retention and Storage Period of Personal Information

- Internal app data (SQLite, local settings, encrypted images): retained on the user's device until the app is deleted, app data is cleared, or the user deletes the data directly
- Temporary files: deleted after the relevant task is completed or cleared according to the operating system's cache policy
- Files exported by the user (PDFs, backup files): may remain in the storage location selected by the user and must be deleted directly by the user
- Advertising/consent-related data (processed by third parties): subject to the policies of each service provider and applicable laws

In principle, the app does not store core user records on the developer's server.  
However, files that the user directly saves to external storage are managed within the user's own environment.

---

## 5. Procedures and Methods for Destruction of Personal Information

When the purpose of processing has been achieved or when the user requests deletion, the app destroys the relevant information or processes it so that it is no longer referenced, as follows.

### 5-1) Destruction Procedures

- When the user directly deletes individual person records, folders, images, backup data, etc., such data is treated as subject to immediate deletion.
- When the user deletes the app or clears app data from device settings, data stored in the app's internal storage area is removed according to the operating system's deletion procedures.
- Temporary files become subject to cleanup after the relevant task ends, and some cached data may remain until a certain point depending on the operating system's policy.

### 5-2) Destruction Methods

- SQLite data: deletion of the relevant records
- App settings (`SharedPreferences`): deletion of the relevant key or all settings
- `flutter_secure_storage` values: deletion of the relevant secure storage items
- Internal app files (encrypted images, temporary files, etc.): deletion of the relevant files
- PDFs/backup files directly saved by the user to external storage: not automatically deleted by the app and must be deleted directly by the user

Unless otherwise required by applicable laws, the developer does not separately store core user records on the developer's server.

---

## 6. Provision to Third Parties, Outsourcing, and Cross-Border Transfer

The app may use Google services for advertising and consent management.

| Item | Details |
|---|---|
| **Recipient / Entrusted Party** | Google LLC and its affiliates (operators of AdMob/UMP) |
| **Country of Transfer** | United States and regions where Google infrastructure is operated |
| **Time of Transfer** | On an ongoing basis during ad requests, consent status checks, SDK initialization, and operation |
| **Method of Transfer** | Transmission through network communication between the app and third-party servers |
| **Legal Basis for Cross-Border Transfer** | Processed within the scope necessary to provide the service under applicable legal grounds, or, where necessary, based on the data subject's consent |
| **Purpose** | Ad serving, ad measurement, consent management, fraud prevention, and compliance with policies/laws |
| **Categories of Data (Examples)** | Advertising identifiers (AAID/IDFA), IP/network information, device/app information, ad interaction information, consent status |
| **Retention Period** | Subject to Google's policies and applicable laws |
| **Effect of Refusal** | Personalized ads may be limited, non-personalized ads may be provided, or some ad-related features may be restricted |

The developer does not collect or sell the app's core people-record data through its own server.

---

## 7. Information on Permissions Used

The app may use the following permissions:

- `INTERNET`: communication for advertising SDKs and related network features
- `com.google.android.gms.permission.AD_ID`: use of advertising identifiers (AdMob)
- `READ_MEDIA_IMAGES` (Android 13+), `READ_EXTERNAL_STORAGE` (Android 12 and below): photo attachment/selection

Permissions are used only within the scope necessary to provide the relevant features.

---

## 8. Installation, Operation, and Refusal of Automatic Collection Mechanisms

This app does not directly operate general website cookies.  
However, in connection with advertising and consent management features, third-party SDKs may automatically process advertising identifiers, network information, device information, and similar data.

Users may adjust the relevant settings in the following ways:

- Change selections within the app's privacy options or consent management screen (where provided)
- Reset or delete the advertising ID in the device operating system settings
- Limit personalized ads or adjust related privacy options in the device operating system settings

If the user limits personalized advertising, non-personalized ads may be provided, or certain ad-related features may be restricted.

---

## 9. User Rights and How to Exercise Them

Subject to applicable laws, users may have the following rights:

- Request access to, correction of, or deletion of personal information
- Request suspension or restriction of processing
- Withdraw consent for consent-based processing
- Change advertising/consent choices

These rights may be exercised in the following ways:

- Directly modify or delete data within the app
- Initialize local data by deleting app data or uninstalling the app
- Change advertising consent through the app's privacy options/consent screen (in regions where provided)
- Reset/delete the advertising ID or limit personalized ads through the device OS settings
- Contact: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

---

## 10. Security Measures

The developer applies or seeks to apply the following measures:

- User records are generally stored locally on the device
- Attached image files are stored locally in encrypted form (AES-GCM based)
- App lock information is stored in hashed form rather than in plain text
- Backup files are stored after being encrypted based on a user password
- Communication with third-party SDKs is encrypted (HTTPS/TLS)
- Permissions are used with minimized scope of access

However, risks arising from the user's device security condition (such as rooting/jailbreaking, malicious apps, or exposure of shared storage) cannot be completely eliminated.

---

## 11. Information Regarding Sensitive Information

This app does not require the input of sensitive information.  
Users are advised not to enter sensitive content such as health information, political opinions, religion, biometric information, or information related to sexual life in notes or free-input fields.

If a user voluntarily enters sensitive content, such information may be stored as local data on the device managed directly by the user.

---

## 12. Protection of Children's Personal Information

This app is not designed primarily for children.  
Guardians may manage usage through parental control features provided by the device or app store.

---

## 13. Automated Decision-Making

This app does not perform automated decision-making based on personal information that produces legal effects or similarly significant impacts.

---

## 14. Data Safety Notice (Google Play, etc.)

The developer strives to maintain and update the data safety disclosure items in app marketplaces (such as Google Play) in accordance with the app's actual processing practices and the actual processing practices of third-party SDKs.

However, the information displayed in app stores may vary depending on the app version, distribution country, third-party SDK configuration, and policy changes.

---

## 15. Open Source Notice

The app uses certain open-source libraries.  
Information on the relevant licenses may be found in the related screen within the app or in notices provided through the distribution channel.

---

## 16. Contact

For inquiries regarding this Privacy Policy:

- **Personal Information Protection Officer / Contact Person:** frog-im
- **Email:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

---

## 17. Changes to This Privacy Policy

This Policy may be revised due to changes in laws/policies, app features, or third-party SDKs.  
If there are material changes, notice may be provided through in-app notices, the distribution page, or updates to the policy page.

Last Updated: **2026-03-04**