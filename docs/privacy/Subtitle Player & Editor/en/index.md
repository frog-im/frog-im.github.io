---
title: Privacy Policy | Subtitle Tool
description: Subtitle Tool (Subtitle Player & Editor) Privacy Policy (English)
lang: en
last_updated: 2025-12-12
---

# Privacy Policy (Subtitle Tool / Subtitle Player & Editor)

- **App name:** Subtitle Player & Editor (also referred to as **“Subtitle Tool”** in this Policy)  
- **Developer:** frog-im  
- **Contact:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)  
- **Effective date:** 2025-12-12  

> This Policy is drafted with reference to applicable laws including the Korean Personal Information Protection Act (PIPA), the GDPR/UK GDPR, the Swiss FADP, and relevant U.S. state privacy laws. If there are jurisdiction-specific requirements, those requirements take precedence.

---

## 1. Purpose and Scope

This app provides:

- **Subtitle playback and editing** (e.g., SRT, VTT, ASS, SSA, LRC)  
- **Video + subtitle playback** from files selected by the user  
- **Floating subtitle / lyrics overlay** displayed over other apps (Android)

The app does **not** create a user account and does **not** upload user media or subtitle content to our own servers.  
Processing is performed **on the user’s device** by default.

However, for **advertising**, **consent management**, and **legal compliance** purposes, third-party partners (such as **Google Mobile Ads SDK (AdMob)** and **Google UMP**) may collect and process information including **advertising identifiers** and related signals.  
Consent collection and privacy choices follow the **Google UMP (User Messaging Platform)** specifications where applicable.

---

## 2. Categories of Information We Process

### 2-1) Files Explicitly Chosen by the User

The app interacts only with **files the user explicitly selects**, such as:

- **Subtitle files**  
  - Examples: `.srt`, `.vtt`, `.ass`, `.ssa`, `.lrc`  
  - **Use:**  
    - Displaying subtitles/lyrics in a floating overlay or inside the app  
    - Editing subtitle timing and text and saving to a new file  
  - **Processing:** Performed **locally on the device** (parsing and saving via libraries such as `subtitle`)

- **Media files (optional)**  
  - Examples: local video/audio files selected by the user (e.g., via file picker)  
  - **Use:** Playing video/audio together with selected subtitles inside the app  
  - **Processing:** Decoding and playback are done **locally** (e.g., using `better_player` or similar libraries)

> **Important:**  
> - The app does **not** upload user-selected subtitles or media files to our own servers.  
> - Paths and contents are used strictly for playback, overlay display, and user-initiated editing.

### 2-2) Local Settings and Stored Values

For the app to function and provide a consistent user experience, certain settings are stored **locally on the device** using `SharedPreferences` or equivalent OS mechanisms.

These values are **not** sent to our own servers and are **removed when the app or its data is deleted**.

#### (1) Overlay position, size, and style (`SharedPreferences`)

| Type | Key (example) | Purpose | Storage | Deletion |
|---|---|---|---|---|
| Overlay position (Y) | `overlay_box_y` | Restore vertical position of subtitle overlay box | Device SharedPreferences | Removed when app data or app is deleted |
| Overlay position (X / left alignment) | `overlay_box_x` | Horizontal alignment / offset (typically fixed or 0) | Same | Same |
| Overlay font size | `overlay_text_font` | Keep user-selected subtitle font size for both overlay and in-app player | Same | Same |
| Overlay font color | `overlay_text_color` | Keep text color for overlay | Same | Same |
| Overlay outline usage | `overlay_outline_enabled` | Whether to draw outline around overlay text | Same | Same |
| Overlay outline color | `overlay_outline_color` | Color of the text outline | Same | Same |
| Overlay outline width | `overlay_outline_width` | Thickness of the text outline | Same | Same |
| Overlay width/height | `overlay_box_w`, `overlay_box_h` | Default or user-tuned overlay size in dp | Same | Same |
| Overlay ad counter | `overlay_interstitial_count` | Internal counter for showing ads periodically (e.g., every 3rd overlay launch) | Same | Same |

These keys are used to:

- Restore the last used overlay position on the screen  
- Synchronize subtitle style between **Overlay Box Editor**, **video player**, and **Android overlay app**  
- Control how often full-screen or rewarded ads are **attempted** (e.g., “every third overlay usage”)

#### (2) Ads / privacy-related preferences

Depending on your region and app settings, the app may store flags such as:

- `pref_npa_always` (non-personalized ads preference)  
- `pref_us_rdp` (U.S. Restricted Data Processing)  
- `pref_child_directed` / `pref_under_age` (child-directed / age-related tagging for ads)  
- `pref_max_ad_rating` (maximum allowed ad content rating)

**Purpose:**  
- To remember your privacy and ad-related choices, and to configure AdMob / UMP in a way that respects those choices.

**Storage / deletion:**  
- Stored locally through `SharedPreferences`.  
- Removed when app data is cleared or the app is uninstalled.

#### (3) Temporary files

During normal operation, the app may create **temporary files**, for example:

- Parsed/converted subtitle contents used internally  
- Small caches created by third-party libraries or file pickers

These temporary files:

- Reside in OS-managed cache or temporary folders  
- Are deleted by the app where practical, and may also be cleaned up by the OS over time  
- Are **not** uploaded to our own servers

#### (4) User-selected save locations

When you use “Save As” or similar features:

- The app may **write subtitle files** to a directory you choose (e.g., Downloads or another folder chosen via a system file picker).  
- Such files reside in **external or user-managed storage** and may **remain after app deletion**.  
- You can delete these files manually via your file manager or cloud storage interface.

#### (5) Consent State (UMP SDK Cache)

In certain regions (EEA/UK/CH and others as determined by Google UMP):

- The **UMP SDK** may cache your ad consent state locally on the device.  
- This can typically be reset by:
  - Clearing the app’s data, or  
  - Using an in-app **Privacy Options / Consent** screen where provided.

---

### 2-3) Ads, Consent, and Related Data (Third-party SDKs)

The app uses **Google Mobile Ads SDK (AdMob)** and **Google UMP** for:

- Displaying ads (including **rewarded ads** for some operations such as subtitle saving)  
- Managing ad-related consent where required by law

These third-party SDKs may collect or process, for example:

- **Advertising identifiers** (e.g., AAID / IDFA)  
- **IP-based information**, approximate location, and general network info  
- Device and app information (OS version, app version, language, crash logs relevant to ads)  
- Ad interaction and engagement signals (e.g., impressions, clicks, completed views in rewarded ads)  
- Consent choices recorded via UMP

**Purposes:**

- Ad delivery and reporting  
- Frequency capping  
- Fraud and abuse prevention  
- Legal compliance (e.g., consent and age-related flags)

Regions such as **EEA/UK/CH**:

- Consent is requested through **UMP prompts** where required.  
- A **Privacy Options** button may be shown to revisit your choices.

Regions without such explicit legal requirements (e.g., Korea):

- The UI may **not** show a separate Privacy Options button if not required,  
  but OS-level settings (e.g., ad ID reset) remain available.

---

## 3. Processing and Retention

- **Local settings (SharedPreferences):**  
  - Retained on the device until you clear app data or uninstall the app.

- **Temporary files:**  
  - Created and used during subtitle operations and playback.  
  - Deleted where practical by the app; also subject to OS-level cache cleanup.

- **User-saved subtitle files:**  
  - Written to destinations you choose (e.g., Downloads, other folders, or cloud locations).  
  - Remain under your control, and are **not removed automatically** when uninstalling the app.

- **Ads / consent data (third-party):**  
  - Stored, processed, and retained in accordance with **Google’s policies** and applicable law.

---

## 4. Third-party Transfers and Cross-Border Data Flows

For advertising and consent management, certain data is processed by **Google** and its partners.

| Item | Details |
|---|---|
| **Recipient** | Google LLC and its affiliates/sub-processors |
| **Destination** | The United States and other regions where Google’s infrastructure is located |
| **Purpose** | Ad delivery, performance measurement, fraud prevention, consent management, and legal compliance |
| **Data** | Advertising identifiers, IP-based info, device/app info, ad interaction signals, consent state, etc. |
| **Retention** | Per Google’s policies and applicable laws |
| **Effect of refusal** | Personalized ads may be limited; non-personalized ads or fewer ads may be shown |

We aim to keep our **Google Play Data safety** disclosures consistent with how the app and its SDKs actually process data.

---

## 5. Your Rights and How to Exercise Them

Depending on your jurisdiction, you may have rights such as:

- Access to your personal data  
- Rectification or erasure  
- Restriction of processing  
- Data portability  
- Objection to certain processing  
- Withdrawal of consent (where consent is the legal basis)

**In practice:**

- **Ads and consent choices**  
  - In UMP-supported regions (e.g., EEA/UK/CH): adjust choices in **Settings → Privacy Options** (if provided in the app UI).  
  - Otherwise, use OS settings to **reset the advertising ID** or limit ad personalization.

- **Local settings and overlay configuration**  
  - Clearing app data or uninstalling the app resets:  
    - Overlay coordinates and size  
    - Font size, color, outline settings  
    - Stored ad/privacy preferences

For ad-related data processed by Google, please refer to and use **Google’s own tools and processes** (e.g., Google account ad settings, UMP dialog, etc.).

---

## 6. Children’s Privacy

This app is **not directed to children**.

- The app’s primary purpose is **subtitle/lyrics editing and floating overlay**, which presumes use by older teens or adults.  
- If a child under the legally required minimum age uses the app, they should stop using it and use OS-level ad-limiting features with a guardian.  

Where appropriate, the developer may enable **child-directed flags (e.g., TFUA)** or equivalent settings in ad SDKs to better protect minors, in line with platform policies.

---

## 7. Security Measures

Within the app’s architecture and scope, we seek to:

- Minimize data collection to what is necessary for subtitle and overlay functionality  
- Keep processing **on-device** wherever possible  
- Limit file access strictly to files you explicitly choose through system file pickers  
- Use **system-level permissions** transparently (e.g., overlay permission, notification permission on Android)  
- Rely on **TLS or equivalent encryption in transit** for network traffic handled by third-party SDKs (such as ad and consent frameworks)

---

## 8. Data Safety (Google Play)

For distribution through app stores such as **Google Play**, we:

- Prepare and maintain a **Data safety** section that accurately reflects how the app and its third-party SDKs handle data  
- Update the disclosure without undue delay if there are material changes in processing (e.g., enabling analytics or crash reporting SDKs in future versions)

---

## 9. Open-source Notices

This app uses open-source software (for example, libraries for:

- Subtitle parsing and serialization  
- Video playback  
- Overlay windows  
- WebView integrations  
- Localization and UI components)

Open-source licenses and notices are provided **inside the app** (e.g., in an “Open Source Licenses” section).  
Where required, source code access instructions for relevant components will be provided in the corresponding notice files.

---

## 10. Contact

If you have questions about this Policy or privacy-related requests:

- **Email:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

Please include the app name **“Subtitle Player & Editor (Subtitle Tool)”** in your inquiry so we can identify the correct app.

---

## 11. Changes to This Policy

We may update this Policy due to:

- Changes in laws or regulations  
- Updates to app features (for example, adding new SDKs or services)  
- Internal policy adjustments

**Minor updates:**  
- Will be posted within the in-app privacy section and on the policy page.

**Material changes:**  
- We will provide notice **at least 7 days before** the new effective date, where required by law or platform policy.
