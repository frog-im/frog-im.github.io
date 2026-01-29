---
title: Patakaran sa Privacy | Power lucky lotto
description: Patakaran sa Privacy ng Power lucky lotto (Filipino)
lang: fil
last_updated: 2026-01-29
---

# Patakaran sa Privacy (Power lucky lotto)

- **Pangalan ng app:** Power lucky lotto  
- **Developer:** frog-im  
- **Contact:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)  
- **Petsa ng bisa:** 2026-01-29  

> Ang patakarang ito ay ginawa bilang sanggunian sa mga naaangkop na batas sa privacy tulad ng Korea PIPA, GDPR/UK GDPR, Swiss FADP, at mga kaugnay na batas sa privacy ng ilang estado sa U.S.  
> Kung may partikular na sapilitang (mandatory) na kinakailangan sa inyong rehiyon, iyon ang masusunod.

---

## 1. Layunin at saklaw

Ang Power lucky lotto ay isang app para sa pamamahala ng mga larong lottery at pagtingin ng mga record. Kabilang sa mga pangunahing feature ang:

- Pagpili ng bansa/laro at setup (hal., KR 6/45, US Powerball)  
- Pagbuo/pag-save ng mga numero at pagtingin ng log (history)  
- Pagtingin at pag-delete ng mga log table (table list/detail)  
- Pag-edit/pamamahala ng game result data gamit ang JSON (para sa stats/visualization)  
- Mga ad (kabilang ang rewarded ads) at consent management (kung kinakailangan)

Ang app ay **hindi nangangailangan ng account** at, sa default, **hindi nag-a-upload ng inyong data sa server ng developer.**  
Karamihan ng pagproseso ay nangyayari **sa inyong device**.

Gayunman, para sa **advertising**, **consent management**, at **legal compliance**, maaaring mangolekta at magproseso ng ilang data ang mga third-party SDK tulad ng  
**Google Mobile Ads SDK (AdMob)** at **Google UMP (User Messaging Platform)** (hal., advertising identifiers).

---

## 2. Mga uri ng data na pinoproseso

### 2-1) Data na naka-store sa inyong device (local storage)

Nag-iimbak ang app ng ilang data **lokal sa inyong device** para magbigay ng feature at mapabuti ang usability.  
Karaniwan, ang data na ito ay **hindi ipinapadala sa server ng developer** at natatanggal kapag dinelete ninyo ang app data o in-uninstall ang app (maliban sa mga file na in-export ninyo sa ibang lugar).

#### (1) Settings (SharedPreferences)

| Category | Key (example) | Purpose | Storage | Deletion |
|---|---|---|---|---|
| Setup completed | `setup_done` | I-store ang initial setup state | SharedPreferences | Tinatanggal sa app data delete/uninstall |
| Country history | `selected_countries` | I-keep ang recently selected countries | Same | Same |
| Active country | `active_country` | I-store ang kasalukuyang selected country | Same | Same |
| Selected games | `selected_lotto_ids` | I-store ang checked game IDs | Same | Same |
| Active game | `active_lotto_id` | I-store ang active game ID | Same | Same |
| **Seed time selection (optional)** | `birth_datetime_iso` | I-store ang seed reference time na pinili ng user (maaaring gamitin para sa seeding/personalization) | Same | Same |

> **Note:** Ang “Seed time selection (optional)” ay pinoproseso lamang kung pinili ng user na i-set ito at maaaring hindi kailangan para sa core app use.

#### (2) Log data (SQLite)

Maaaring mag-store ang app ng generated/saved records sa local SQLite database.

- Example tables: `log_...`  
- Example fields:  
  - `id`, `date_id` o `date_text` (timestamp), `choice1..choiceN` (picked numbers), `isFinger` (fingerprint-related flag, atbp.)

Maaari ninyong tingnan ang logs sa table list/detail screens at i-delete ang mga ito (table-level o row-level) kung nais.

#### (3) JSON data files (per game)

Maaaring mag-store ang app ng game-specific JSON data sa documents directory ng app.

- Example: `game_json/<gameId>.json`  
- Purpose: user-managed/editable draw/result data (hal., para sa statistics/visualization)

Ang mga file na ito ay naka-store on-device at karaniwang natatanggal kapag in-uninstall ang app, depende sa OS/backup behavior.

---

### 2-2) Ads, consent, at kaugnay na data (third-party SDKs)

Ginagamit ng app ang **Google Mobile Ads SDK (AdMob)** at **Google UMP** para:

- Magpakita ng ads (kabilang ang **rewarded ads**)  
- Mag-manage ng consent na legal na kinakailangan para sa advertising

Ang mga SDK na ito ay maaaring mangolekta/magproseso ng, halimbawa:

- **Advertising ID** (hal., AAID, IDFA)  
- IP-based info, approximate location, network info  
- Device/app info (OS version, app version, language, diagnostic info)  
- Ad interactions (impressions, clicks, rewarded completion)  
- Consent choices na naitala ng UMP

Sa ilang rehiyon (hal., EEA/UK/CH), maaaring ipakita ang UMP consent form at magbigay ng **Privacy Options** entry kung kinakailangan.

---

## 3. Retention

- **Local settings (SharedPreferences):** naka-keep hanggang app data deletion o uninstall  
- **Log data (SQLite):** naka-keep hanggang i-delete ninyo o i-uninstall/i-clear ang app data  
- **JSON files:** naka-store sa documents directory; madalas natatanggal sa uninstall, pero ang exports/backups ay user-managed  
- **Ads/consent data (third-party):** ayon sa Google policies at applicable laws

---

## 4. Third-party sharing at international transfers

Para sa ads at consent management, maaaring iproseso ang ilang data ng **Google at mga partner nito**.

| Item | Details |
|---|---|
| **Recipients** | Google LLC, affiliates, at subprocessors |
| **Transfer destinations** | United States at iba pang rehiyon kung saan naroon ang Google infrastructure |
| **Purpose** | Ad delivery, measurement, fraud prevention, consent management, compliance |
| **Data** | Advertising ID, IP-based info, device/app info, ad interaction data, consent status |
| **Retention** | Ayon sa Google policies at applicable law |
| **Impact if you decline** | Maaaring ma-limit ang personalized ads; maaaring magpakita ng non-personalized ads o mas kaunting ads |

---

## 5. Mga karapatan ninyo at paano ito gamitin

Depende sa naaangkop na batas, maaari kayong magkaroon ng karapatang tulad ng access, correction, deletion, restriction, objection, portability, at withdrawal of consent (kung consent ang legal basis).

Mga halimbawa:

- **Ayusin ang ads/consent choices:** sa in-app Privacy Options (kung available) o sa OS ad settings (i-reset ang advertising ID, i-limit ang ad personalization).  
- **I-reset ang local data:** i-clear ang app data o i-uninstall ang app para matanggal ang local settings/logs/files na naka-store ng app.

---

## 6. Privacy ng mga bata

Ang app na ito ay **hindi dinisenyo para sa mga bata**. Kung gagamit ang bata, dapat isaalang-alang ng guardian ang OS-level parental controls at ad limitation features.

---

## 7. Security measures

Sa saklaw ng app, nagsusumikap kami na:

- Mag-store lamang ng minimum necessary data locally  
- Panatilihing on-device ang processing kung maaari  
- Umasa sa TLS/secure transport para sa SDK network communications (sa loob ng kakayahan ng SDK)

---

## 8. Google Play Data safety

Kung ipapamahagi sa Google Play, layunin naming panatilihing tama at updated ang Data safety disclosures, lalo na kapag may pagbabago sa SDKs o processing practices.

---

## 9. Open-source notices

Maaaring gumamit ang app ng open-source libraries para sa country icons, storage, ads/consent, at UI.  
Makikita ang license notices sa “Open-source licenses” screen ng app (o katumbas).

---

## 10. Contact

Para sa mga tanong tungkol sa privacy:

- **Email:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

Pakibanggit ang **“Power lucky lotto”** sa inyong mensahe.

---

## 11. Changes sa policy na ito

Maaaring magbago ang policy na ito dahil sa legal updates, feature changes (hal., bagong SDKs), o internal policy adjustments.  
Ang minor changes ay ipo-post sa app o sa page na ito; ang material changes ay iaanunsyo nang mas maaga kung kinakailangan.
