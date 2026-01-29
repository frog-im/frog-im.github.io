---
title: Privacy Policy | Power lucky lotto
description: Power lucky lotto Privacy Policy (English)
lang: en
last_updated: 2026-01-29
---

# Privacy Policy (Power lucky lotto)

- **App name:** Power lucky lotto  
- **Developer:** frog-im  
- **Contact:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)  
- **Effective date:** 2026-01-29  

> This policy is written with reference to applicable privacy laws such as Korea PIPA, GDPR/UK GDPR, Swiss FADP, and relevant U.S. state privacy laws.  
> If your region has specific mandatory requirements, those requirements take precedence.

---

## 1. Purpose and scope

Power lucky lotto is an app for managing lottery games and viewing records. Key features include:

- Country/game selection and setup (e.g., KR 6/45, US Powerball)  
- Number generation/saving and log (history) viewing  
- Viewing and deleting log tables (table list/detail)  
- Editing/managing game result data via JSON (for stats/visualization)  
- Ads (including rewarded ads) and consent management (where required)

The app **does not require account creation** and, by default, **does not upload your data to the developer’s servers.**  
Most processing happens **on your device**.

However, for **advertising**, **consent management**, and **legal compliance**, third-party SDKs such as  
**Google Mobile Ads SDK (AdMob)** and **Google UMP (User Messaging Platform)** may collect and process certain data (e.g., advertising identifiers).

---

## 2. Types of data processed

### 2-1) Data stored on your device (local storage)

The app stores certain data **locally on your device** to provide features and improve usability.  
This data is generally **not transmitted to the developer’s servers** and is removed when you delete app data or uninstall the app (except for files you export elsewhere).

#### (1) Settings (SharedPreferences)

| Category | Key (example) | Purpose | Storage | Deletion |
|---|---|---|---|---|
| Setup completed | `setup_done` | Store initial setup state | SharedPreferences | Removed on app data delete/uninstall |
| Country history | `selected_countries` | Keep recently selected countries | Same | Same |
| Active country | `active_country` | Store the currently selected country | Same | Same |
| Selected games | `selected_lotto_ids` | Store checked game IDs | Same | Same |
| Active game | `active_lotto_id` | Store the active game ID | Same | Same |
| **Seed time selection (optional)** | `birth_datetime_iso` | Store a user-selected seed reference time (may be used for seeding generation/personalization) | Same | Same |

> **Note:** “Seed time selection (optional)” is only collected if the user chooses to set it and may not be required for core app use.

#### (2) Log data (SQLite)

The app may store generated/saved records in a local SQLite database.

- Example tables: `log_...`  
- Example fields:  
  - `id`, `date_id` or `date_text` (timestamp), `choice1..choiceN` (picked numbers), `isFinger` (fingerprint-related flag, etc.)

You can view logs in the app’s table list/detail screens and delete them (table-level or row-level) if you wish.

#### (3) JSON data files (per game)

The app may store game-specific JSON data in the app’s documents directory.

- Example: `game_json/<gameId>.json`  
- Purpose: user-managed/editable draw/result data (e.g., for statistics/visualization)

These files are stored on-device and are generally removed when the app is uninstalled, subject to OS/backup behavior.

---

### 2-2) Ads, consent, and related data (third-party SDKs)

The app uses **Google Mobile Ads SDK (AdMob)** and **Google UMP** to:

- Show ads (including **rewarded ads**)  
- Manage legally required consent for advertising

These SDKs may collect/process, for example:

- **Advertising ID** (e.g., AAID, IDFA)  
- IP-based info, approximate location, network info  
- Device/app info (OS version, app version, language, diagnostic info)  
- Ad interactions (impressions, clicks, rewarded completion)  
- Consent choices recorded by UMP

In some regions (e.g., EEA/UK/CH), a UMP consent form may be shown and a **Privacy Options** entry may be provided where required.

---

## 3. Retention

- **Local settings (SharedPreferences):** kept until app data deletion or uninstall  
- **Log data (SQLite):** kept until you delete it or uninstall/clear app data  
- **JSON files:** stored in the app’s documents directory; removed on uninstall in many cases, but user exports/backups are user-managed  
- **Ads/consent data (third-party):** retained according to Google policies and applicable laws

---

## 4. Third-party sharing and international transfers

For ads and consent management, some data may be processed by **Google and its partners**.

| Item | Details |
|---|---|
| **Recipients** | Google LLC, affiliates, and subprocessors |
| **Transfer destinations** | United States and other regions where Google infrastructure is located |
| **Purpose** | Ad delivery, measurement, fraud prevention, consent management, compliance |
| **Data** | Advertising ID, IP-based info, device/app info, ad interaction data, consent status |
| **Retention** | Per Google policies and applicable law |
| **Impact if you decline** | Personalized ads may be limited; non-personalized ads or fewer ads may be shown |

---

## 5. Your rights and how to exercise them

Depending on applicable law, you may have rights such as access, correction, deletion, restriction, objection, portability, and withdrawal of consent (where consent is the legal basis).

Examples:

- **Adjust ads/consent choices:** via in-app Privacy Options (where available) or OS ad settings (reset advertising ID, limit ad personalization).  
- **Reset local data:** clear app data or uninstall the app to remove local settings/logs/files stored by the app.

---

## 6. Children’s privacy

This app is **not designed for children**. If a child uses the app, a guardian should consider using OS-level parental controls and ad limitation features.

---

## 7. Security measures

Within the app’s scope, we strive to:

- Store only the minimum necessary data locally  
- Keep processing on-device where possible  
- Rely on TLS/secure transport for SDK network communications (within SDK capabilities)

---

## 8. Google Play Data safety

If distributed on Google Play, we aim to keep Data safety disclosures accurate and updated, especially when SDKs or processing practices change.

---

## 9. Open-source notices

The app may use open-source libraries for country icons, storage, ads/consent, and UI.  
License notices are available in the app’s “Open-source licenses” screen (or equivalent).

---

## 10. Contact

For privacy inquiries:

- **Email:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

Please mention **“Power lucky lotto”** in your message.

---

## 11. Changes to this policy

This policy may change due to legal updates, feature changes (e.g., new SDKs), or internal policy adjustments.  
Minor changes will be posted in-app or on this page; material changes will be announced in advance as required.
