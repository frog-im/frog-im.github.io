---
title: Privacy Policy | FileGuard
description: FileGuard Privacy Policy
lang: en
last_updated: 2026-06-23
---

# Privacy Policy (FileGuard)

- **App:** FileGuard
- **Developer:** frog-im
- **Privacy contact:** frog-im
- **Email:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- **Effective date:** June 23, 2026
- **Last updated:** June 23, 2026

> This Policy describes the current implementation of the FileGuard app. Mandatory laws in your country or region may take precedence.

---

## 1. Scope and purpose

FileGuard is a security utility that lets you keep selected files, captured media, notes, and clipboard text in encrypted vaults on your device and create encrypted backup files.

The app does not require registration or sign-in. The developer does not operate a server that receives your vault files, file contents, passwords, vault names, or activity history. On Android, however, the app may use Google AdMob and Google User Messaging Platform (UMP) for advertising and privacy choices.

## 2. Information processed

### 2.1 Vault data selected or created by you

The app may process the following information on your device:

- Photos, videos, documents, and other files you select through the system file picker
- Photos or videos captured with the app, including audio recorded with a video
- Clipboard text that you save manually or that is detected when you enable automatic clipboard protection
- File name, MIME type, size, creation time, caption, and preview-related information
- Vault name and identifier, security classification, original-file status, and original-file reference
- Encrypted export, transfer, or backup packages you create

This information is processed on your device to provide the app's features. The developer does not upload it to a developer-operated server.

### 2.2 Authentication and security information

The app may process the following information in secure storage on your device:

- Salts, key-derivation settings, and encrypted key bundles used to derive or protect encryption keys
- Vault access credentials and local keys protected by a device-bound key for biometric access
- Security preferences such as screenshot protection, clipboard clearing, biometric reauthentication, and automatic protection

Your plaintext password is not sent to the developer. Biometric authentication is performed by the operating system. The app does not collect fingerprint or face images or biometric templates; it receives only the authentication result.

### 2.3 Local activity and backup information

The app may locally store:

- The type, description, time, and related item identifiers for protection, locking, deletion, original deletion, backup, and restore events
- Up to 500 activity-log entries
- Backup destination, last backup time, item count, and success or failure status
- Whether automatic backup is enabled and the password required to update that backup
- Ad privacy choices, restricted-data-processing choice, and a protected-item count used for ad frequency

Sensitive settings, including backup state and the automatic-backup password, are stored in a device-key-encrypted local store. You are responsible for keeping your backup password secure.

### 2.4 Information processed during advertising and consent

On the supported advertising platform, currently Android, the app may use Google AdMob and UMP. Google and advertising technology providers may process:

- Advertising, app-instance, or device-related identifiers
- IP address and approximate location inferred from information such as the IP address
- Device model, operating system, app version, language, and network information
- Ad requests, impressions, clicks, interactions, and diagnostics
- Consent status and regional privacy choices

This information may be used for ad delivery, non-personalized ads, frequency capping, measurement, fraud prevention, consent management, security, and legal compliance. The app is implemented to initialize the Google Mobile Ads SDK only after UMP indicates that ads may be requested.

See the [Google Privacy Policy](https://policies.google.com/privacy) and [Google advertising technologies information](https://policies.google.com/technologies/ads).

## 3. Purposes of processing

FileGuard processes information to:

- Store and display selected or captured content in encrypted vaults
- Control vault access with locking, passwords, and biometric authentication
- Import, export, move, delete, and track the original-file status of content
- Create and restore encrypted backups at a location selected by you
- Maintain security preferences and clear temporary decrypted files and clipboard contents
- Display local security activity and error status
- Deliver Android ads, control ad frequency, and provide privacy choices
- Prevent abuse, secure the service, and comply with legal obligations

## 4. Storage and retention

| Category | Storage and retention | How to delete |
|---|---|---|
| Encrypted vault files and metadata | Stored in app-private local storage until you delete them | Delete the item or vault in the app, clear app data, or uninstall |
| Credentials and security settings | Stored in operating-system secure storage and device-key-encrypted storage until changed or app data is removed | Disable the relevant feature, clear app data, or uninstall |
| Activity history | Up to 500 entries in encrypted local storage | Clear app data or uninstall |
| Temporary decrypted files | Temporarily written to app cache and cleared on startup, backgrounding, or feature completion on a best-effort basis | Close the app or clear its cache/data |
| Clipboard content | Processed through the operating-system clipboard when copy or automatic protection is used | Automatic best-effort clearing, copy other content, or restart the device |
| Encrypted backup files | Stored in a device folder, document provider, or cloud-synced location selected by you until you delete them | Delete through the relevant file manager or storage service |
| Google advertising data | Retained under Google and processor policies and legal obligations | Change app/device ad settings or use Google privacy controls |

The operating system, device manufacturer, document provider, or cloud backup provider may keep separate copies of app data or backup files you create. Those copies are governed by the relevant provider's policies.

## 5. Third parties, service providers, and sale

The developer does not sell vault content, passwords, or in-app activity history and does not provide them to third parties through a developer-operated server.

When Android advertising or consent features operate, Google LLC, Google affiliates, advertising technology providers, and related processors may process the information described in Section 2.4. See the separate [International Data Transfer Notice](policy/).

If you directly select an external app or cloud service through a file picker, sharing function, or backup destination, that provider may process files at your direction. Its privacy policy and security settings apply, and the developer does not control the provider's practices.

## 6. International data transfers

Vault content is not transferred to a developer-operated server. Advertising and consent information may be processed by Google and related processors in the United States and other countries where they operate infrastructure.

If you choose an overseas cloud service as the location for an encrypted backup, the file may be synchronized to servers outside your country at your direction. See the [International Data Transfer Notice](policy/) for details.

## 7. Permissions

The app may use the following permissions or system capabilities when you use the relevant feature:

- **Files and photos:** Import only content that you select
- **Camera:** Capture photos or videos for the vault
- **Microphone:** Include audio when recording video
- **Biometrics:** Confirm vault access or sensitive settings changes
- **Internet and network state on Android:** Request AdMob ads and UMP consent information
- **Advertising ID on Android:** Support Google advertising features
- **Clipboard:** Copy content or protect clipboard text when you explicitly enable automatic protection

Denying a permission may disable only the related feature. When the system file picker is used, access is generally limited to items you select.

## 8. Security measures and limitations

The current implementation uses measures that include:

- AES-256-GCM encryption for vault content and vault indexes
- PBKDF2-HMAC-SHA256 key derivation for password-based keys
- Android Keystore or StrongBox protection for local keys on supported Android devices
- Device-key encryption for sensitive settings and activity history
- Best-effort vault locking and temporary-file and clipboard cleanup when the app enters the background
- Optional screenshot protection and biometric reauthentication
- Password-encrypted portable backup packages

No security method eliminates every risk. Device theft, malware, operating-system vulnerabilities, weak passwords, files shared by you, or security issues at an external storage provider may expose information.

Opening or exporting decrypted content to another app may create a separate copy. Original-file deletion and temporary-file or clipboard cleanup may be restricted by the operating system, so you should verify the removal of sensitive content.

## 9. Your rights and choices

Most information remains only on your device, so the developer cannot remotely access, correct, or delete it. You can:

- Delete vault items or vaults in the app
- Change security, biometric, automatic-protection, clipboard, and automatic-backup settings
- Clear app data or cache, or uninstall the app
- Delete backup and exported files from their storage location
- Where available, change consent through Google's ad privacy options in the app
- Delete or reset the advertising identifier or limit ad personalization in device settings

You may contact us regarding information you directly provided to the developer, such as an inquiry email. Where applicable, local law may give you rights of access, correction, deletion, restriction, withdrawal of consent, and complaint to a supervisory authority.

## 10. Children

FileGuard is not designed primarily for children and does not require children to provide personal information. Guardians may use parental controls provided by the device or app store. The under-age consent configuration for Android advertising should be separately reviewed against the intended audience and applicable law before distribution.

## 11. Contact

For questions about this Policy:

- **Contact:** frog-im
- **Email:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

For advertising data processed by Google, use the privacy controls and contact procedures described in the [Google Privacy Policy](https://policies.google.com/privacy).

## 12. Changes to this Policy

We may update this Policy when laws, app features, permissions, or third-party SDK practices change. Material changes may be communicated on this page, in the app, or through the distribution page.

Last updated: **June 23, 2026**
