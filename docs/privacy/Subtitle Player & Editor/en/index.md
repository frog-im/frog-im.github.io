---
title: Privacy Policy | Subtitle Tool
description: Subtitle Tool (Subtitle Player & Editor) Privacy Policy (English)
lang: en
last_updated: 2026-03-11
---

# Privacy Policy (Subtitle Tool / Subtitle Player & Editor)

- **App name:** Subtitle Player & Editor (also referred to as **Subtitle Tool** in this Policy)
- **Developer:** frog-im
- **Contact:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- **Effective date:** 2026-03-11

> This Policy is prepared with reference to applicable laws including the Korean Personal Information Protection Act (PIPA), the GDPR / UK GDPR, the Swiss FADP, and relevant U.S. state privacy laws. If mandatory local rules apply, those rules take precedence.

---

## 1. Purpose and Scope

This app provides:

- Subtitle playback and editing
- Video + subtitle playback from files selected by the user
- Floating subtitle / lyrics overlay shown over other apps on Android

Supported subtitle handling may include formats such as:

- `srt`
- `vtt`
- `ass`
- `ssa`
- `lrc`
- `txt`

The app does **not** create a user account and does **not** upload user subtitle or media files to the developer's own servers. Subtitle parsing, editing, previewing, and most playback-related processing are performed **locally on the device**.

However, for advertising, consent management, and legal compliance, third-party SDKs such as **Google Mobile Ads SDK (AdMob)** and **Google UMP** may process certain information such as advertising identifiers, device signals, and consent choices.

---

## 2. Categories of Information We Process

### 2-1) Files Explicitly Chosen by the User

The app interacts with files the user explicitly selects, including:

- **Subtitle files**
  - Examples: `.srt`, `.vtt`, `.ass`, `.ssa`, `.lrc`, `.txt`
  - Uses:
    - Subtitle playback inside the app
    - Subtitle editing
    - Overlay subtitle display
    - Subtitle conversion and export

- **Media files**
  - Examples: local video or audio files chosen by the user
  - Uses:
    - Video + subtitle playback
    - Overlay timing alignment against currently playing media

Important points:

- User-selected files are processed locally on the device.
- The app does not upload those files to the developer's own servers.
- File paths and contents are used only for playback, overlay, editing, saving, and user-requested actions.

### 2-2) Local Settings and Stored Values

To provide persistent settings and restore prior state, the app stores some values locally on the device using `SharedPreferences` or similar OS-provided local storage.

These values are not sent to the developer's own servers and are normally removed if the app's data is cleared or the app is uninstalled.

#### (1) Overlay settings

Examples include:

- `overlay_box_x`
- `overlay_box_y`
- `overlay_text_font`
- `overlay_text_color`
- `overlay_outline_enabled`
- `overlay_outline_color`
- `overlay_outline_width`
- `overlay_force_landscape`
- `overlay_interstitial_count`

Purpose:

- Restore overlay position
- Restore subtitle style for overlay and in-app subtitle playback
- Keep outline / font / orientation preferences
- Control ad display frequency logic for some overlay-related flows

#### (2) Recent playback or overlay positions

Examples include:

- `overlay_recent_positions`
- `video_subtitle_recent_position`

Purpose:

- Restore or suggest recent subtitle/overlay starting positions
- Resume video + subtitle playback more conveniently

#### (3) Ad and privacy preference values

Examples may include:

- `pref_npa_always`
- `pref_us_rdp`
- `pref_child_directed`
- `pref_under_age`
- `pref_max_ad_rating`

Purpose:

- Store ad privacy choices
- Apply UMP / AdMob privacy and ad configuration settings

#### (4) User-created subtitle output

When the user saves or exports subtitle files, the app may write new subtitle files to a location selected by the user, such as:

- Downloads
- Another folder selected through a system picker
- A user-managed storage location

These user-saved files may remain on the device after app deletion unless the user deletes them manually.

#### (5) Temporary files and caches

The app and third-party libraries may create temporary or cache files for normal operation, such as:

- file picker cache data
- temporary subtitle conversion data
- playback-related cache data

These are intended for local operation only and are not uploaded to the developer's own servers.

#### (6) UMP consent state cache

In regions where Google UMP applies, the SDK may cache consent state locally on the device.

This can generally be reset by:

- clearing app data, or
- changing consent choices inside the app where a privacy options entry is available

### 2-3) Android Overlay and Permission-Related Processing

On Android, the floating subtitle overlay may use:

- `SYSTEM_ALERT_WINDOW` / display-over-other-apps permission
- `POST_NOTIFICATIONS` permission
- a foreground service notification required for the overlay service

Purpose:

- display subtitle overlay above other apps
- keep the overlay service running
- allow Android to show required overlay / service notifications
- read media notification information when needed for subtitle progression support

These permissions are used only for app features the user chooses to use.

### 2-4) Ads, Consent, and Related Data (Third-party SDKs)

The app uses Google ad / consent SDKs, including:

- **Google Mobile Ads SDK (AdMob)**
- **Google UMP**

The app may show:

- banner ads
- interstitial ads
- rewarded or rewarded-interstitial ads

These SDKs may process data such as:

- advertising identifiers (for example, AAID / IDFA where applicable)
- IP-based and network-related information
- device and app metadata
- ad interaction signals
- consent choices

Purposes may include:

- ad delivery
- ad measurement and reporting
- frequency capping
- fraud prevention
- legal compliance

The developer aims to configure these SDKs in a manner consistent with the user's consent choices and applicable law.

---

## 3. How We Process and Retain Data

- **Local settings and recent position data**
  - retained on the device until app data is cleared or the app is removed

- **Temporary files / cache**
  - retained only as needed for operation, then removed by the app where practical or later cleaned by the OS

- **User-saved subtitle files**
  - remain in the save location chosen by the user until deleted by the user

- **Ad / consent data handled by third parties**
  - retained according to Google policies and applicable law

---

## 4. Third-party Processing and Cross-Border Transfers

For ads and consent management, some information may be processed by Google and related partners.

| Item | Details |
|---|---|
| Recipient | Google LLC and related affiliates / processors |
| Purpose | Ad delivery, measurement, fraud prevention, consent management, and legal compliance |
| Possible data | Advertising identifiers, device/app info, IP-based info, ad interaction data, consent state |
| Destination | United States and other regions where Google infrastructure operates |
| Retention | According to Google policies and applicable law |

The developer aims to keep app store privacy disclosures consistent with actual SDK behavior.

---

## 5. Your Rights and Choices

Depending on your jurisdiction, you may have rights such as:

- access
- correction
- deletion
- restriction
- portability
- objection
- withdrawal of consent where consent is the legal basis

Practical controls include:

- changing ad / privacy choices in the app where available
- clearing app data to remove local settings and cached preferences
- uninstalling the app
- deleting exported subtitle files manually from user storage
- using OS-level controls such as notification settings, ad ID reset, or ad personalization settings

For data processed by Google, users should also refer to Google's own privacy and account tools where relevant.

---

## 6. Children's Privacy

This app is not intended primarily for children.

Its main purpose is subtitle playback, editing, overlay display, and related utility features. Where appropriate, ad SDK configuration may apply age-related or child-directed flags consistent with platform requirements and the developer's settings.

---

## 7. Security Measures

Within the limits of the app's architecture, the developer seeks to:

- minimize collection by keeping most subtitle and media processing on-device
- use system file pickers and user-initiated file access
- use system permissions transparently
- rely on encrypted network transport used by third-party SDKs where applicable

No method of storage or transmission is perfectly secure, but the app is designed to avoid unnecessary collection by the developer.

---

## 8. Open-source Software

The app uses open-source software, including libraries related to:

- subtitle parsing and serialization
- file picking
- local preferences
- overlay windows
- video playback
- WebView

Open-source notices are available inside the app. For some components, the app may use a locally modified copy of an open-source package while preserving the original license notice.

---

## 9. Contact

If you have questions or privacy-related requests:

- **Email:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

Please include the app name **Subtitle Player & Editor** in your message.

---

## 10. Changes to This Policy

This Policy may be updated if:

- app features change
- permissions or SDK usage change
- legal or platform requirements change

Material changes will be reflected in the updated policy page and, where appropriate, in the app.

