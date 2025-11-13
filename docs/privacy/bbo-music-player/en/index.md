---
title: Privacy Policy | LyriFloat
description: LyriFloat Privacy Policy (English)
lang: en
last_updated: 2025-10-30
---

# Privacy Policy (LyriFloat)

- **App name:** LyriFloat  
- **Developer:** frog-im  
- **Contact:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- **Effective date:** 2025-10-30

> This Policy is drafted with reference to applicable laws including the Korean Personal Information Protection Act (PIPA), the GDPR/UK GDPR, the Swiss FADP, and relevant U.S. state privacy laws. If there are jurisdiction-specific requirements, those requirements take precedence.

---

## 1. Purpose and Scope

This app provides **editing of audio file metadata** (title, artist, etc.) stored on the device and **lyrics overlay** features.  
The app does **not** create a user account and does **not** upload user content to any server. Processing is performed **on the user’s device** by default.

However, for **advertising** and **legal compliance** purposes, third-party partners (e.g., Google Mobile Ads SDK (AdMob), UMP) may collect and process information such as **advertising identifiers**. Consent collection and privacy choices follow the **Google UMP (User Messaging Platform)** specifications.

---

## 2. Categories of Information We Process

### 2-1) Files Explicitly Chosen by the User
- **Audio/cover image paths and contents:** processed **locally** on the device solely for editing/saving.  
- **FFmpegKit** is used locally for encoding, metadata editing, and thumbnail extraction.  
- The app **does not upload** user-selected files to our servers.

### 2-2) Local Settings and Stored Values

For core functionality and user convenience, the app stores the following values **locally on the device**.  
These values are not sent to our servers and are **removed when the app or its data is deleted**.

#### (1) Preferences (`shared_preferences`)
| Type | Key/Content | Purpose | Storage | Deletion |
|---|---|---|---|---|
| Overlay position/font | `overlay_box_x`, `overlay_box_y`, `overlay_text_font` | Restore overlay position and font size | Device SharedPreferences | Removed when app data or app is deleted |
| Ads/Privacy settings | `pref_npa_always`, `pref_us_rdp`, `pref_child_directed`, `pref_under_age`, `pref_max_ad_rating` | Non-personalized ads, U.S. RDP, COPPA tag, age tag, ad content rating limit | Device SharedPreferences | Same as left |

#### (2) Temporary Files (system temp directory)
- **Examples:** `cover_*.jpg`, `tmp_*.flac`  
- **Use:** cover art extraction, FLAC tagging, temporary encoding  
- **Location:** OS temporary folder (`systemTemp`)  
- **Retention:** removed by the app after completion when possible; also subject to OS cleanup

#### (3) User-selected Save (SAF)
- When the user chooses “Save As,” final audio files may be written to user-designated locations (e.g., Downloads, cloud).  
- These files reside in **external storage** and **remain after app deletion**. The user can delete them manually.

#### (4) Consent State (UMP SDK Cache)
- In EEA/UK/CH regions, UMP SDK **caches the user’s ad consent state locally**.  
- It can be reset via app data deletion or from the in-app **Privacy Options** screen where available.

---

### 2-3) Ads and Consent-Related Data (Third-party SDKs)
- **Google Mobile Ads SDK (AdMob) and UMP** may collect/process, for example: **advertising identifiers (AAID/IDFA)**, **IP ranges**, **device/app info**, **ad interaction signals**, **consent state**, etc.  
- **Purposes:** ad delivery, frequency capping, fraud prevention, performance measurement, legal compliance  
- **Regions requiring consent (EEA/UK/CH):** consent is collected via UMP prompts, and a **Privacy Options** screen is provided when required.  
  In regions without such requirements (e.g., KR), the option **may not be shown**.

---

## 3. Processing and Retention

- **Local settings:** stored on the device until the user deletes app data or uninstalls the app  
- **Temporary files:** created during encoding/extraction, deleted after processing or may temporarily remain in OS caches  
- **Ads/consent data (third-party):** retained and disposed of in accordance with **Google’s policies**

---

## 4. Third-party Transfers and Cross-Border Data Flows

For advertising and consent management, user information may be transmitted to and processed on Google infrastructure.

| Item | Details |
|---|---|
| **Recipient** | Google LLC and its affiliates/sub-processors |
| **Destination** | The United States (and other regions where Google infrastructure is located) |
| **Purpose** | Ad delivery, performance/measurement, legal compliance, consent management |
| **Data** | Advertising identifiers, IP ranges, device/app info, ad interactions, consent state, etc. |
| **Retention** | Per Google’s policies |
| **Effect of Refusal** | Personalized ads may be limited; non-personalized ads may be shown |

We comply with the **Google Play Data safety** disclosure requirements and keep disclosures aligned with actual processing.

---

## 5. Your Rights and How to Exercise Them

- **Opt out of personalized ads / change consent**  
  - In supported regions (EEA/UK/CH): change preferences in **Settings → Privacy Options**.  
  - Other regions: use the OS settings to **reset ad IDs / limit ad tracking**.
- **Reset local information:** deleting app data or uninstalling the app resets overlay coordinates, font size, and other local settings.
- Rights under **GDPR/UK GDPR/Swiss FADP/U.S. state privacy laws** (access, rectification, erasure, portability, restriction, withdrawal of consent, etc.) can be exercised as provided by those laws.  
  For ad-related data processed by Google, please use **Google’s processes**.

---

## 6. Children’s Privacy

This app **is not directed to children**. If a child under the legal minimum age uses the app, they should stop and use OS-level ad-limiting features with a guardian. When appropriate, we may apply **TFUA (child-directed tag)** or similar child-protection options.

---

## 7. Security Measures

- **Data minimization** in collection and storage  
- **Limited use** of temporary files and deletion attempts after processing  
- Processing strictly **within OS permission scope**  
- **TLS or equivalent** encryption in transit for third-party transfers (per third-party SDK standards)

---

## 8. Data Safety (Google Play)

We prepare and maintain the **Data safety** section in the Play Console accurately, and update it promptly upon changes.

---

## 9. Open-source Notices

The app uses open-source software such as **FFmpeg**. An information file (e.g., `open-source/ffmpeg/WHERE-TO-GET-SOURCE.txt`) within the app explains how to obtain source code. Upon request, we will provide the source as instructed in that file.

---

## 10. Contact

- Email: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

---

## 11. Changes to This Policy

We may revise this Policy due to legal or service changes. We will post updates **in-app** and on this **policy page**.  
For material changes, we will provide notice **at least 7 days before** the effective date.

---

## Appendix: User Guidance

- **In-app link:** open this page from **Settings → Privacy**.  
- **Regional behavior:** in EEA/UK/CH, Privacy Options are shown. **In KR and some other regions, the button may not show additional options** where not legally required.



