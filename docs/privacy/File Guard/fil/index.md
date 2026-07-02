---
title: Patakaran sa Privacy | FileGuard
description: Patakaran sa Privacy ng FileGuard
lang: fil
last_updated: 2026-06-23
---

# Patakaran sa Privacy (FileGuard)

- **App:** FileGuard
- **Developer:** frog-im
- **Contact sa privacy:** frog-im
- **Email:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- **Petsa ng bisa:** Hunyo 23, 2026
- **Huling na-update:** Hunyo 23, 2026

> Inilalarawan ng Patakarang ito ang kasalukuyang implementasyon ng FileGuard app. Maaaring mangibabaw ang mga sapilitang batas sa iyong bansa o rehiyon.

---

## 1. Saklaw at layunin

Ang FileGuard ay isang security utility na nagbibigay-daan sa iyo na itago ang mga napiling file, nakuhang media, tala, at teksto sa clipboard sa mga naka-encrypt na vault sa iyong device at gumawa ng mga naka-encrypt na backup file.

Hindi nangangailangan ang app ng pagpaparehistro o pag-sign in. Hindi nagpapatakbo ang developer ng server na tumatanggap ng iyong mga vault file, nilalaman ng file, password, pangalan ng vault, o kasaysayan ng aktibidad. Gayunpaman, sa Android, maaaring gamitin ng app ang Google AdMob at Google User Messaging Platform (UMP) para sa advertising at mga pagpipilian sa privacy.

## 2. Impormasyong pinoproseso

### 2.1 Data ng vault na pinili o ginawa mo

Maaaring iproseso ng app ang sumusunod na impormasyon sa iyong device:

- Mga larawan, video, dokumento, at iba pang file na pinili mo sa pamamagitan ng system file picker
- Mga larawan o video na kinunan gamit ang app, kasama ang audio na na-record sa isang video
- Teksto sa clipboard na manu-mano mong sine-save o nade-detect kapag pinagana mo ang awtomatikong proteksyon ng clipboard
- Pangalan ng file, MIME type, laki, oras ng paggawa, caption, at impormasyong kaugnay ng preview
- Pangalan at identifier ng vault, klasipikasyon ng seguridad, status ng orihinal na file, at reference ng orihinal na file
- Mga naka-encrypt na export, transfer, o backup package na ginagawa mo

Pinoproseso ang impormasyong ito sa iyong device upang maibigay ang mga feature ng app. Hindi ito ina-upload ng developer sa server na pinapatakbo ng developer.

### 2.2 Impormasyon sa authentication at seguridad

Maaaring iproseso ng app ang sumusunod na impormasyon sa secure storage sa iyong device:

- Mga salt, key-derivation setting, at naka-encrypt na key bundle na ginagamit upang bumuo o protektahan ang encryption keys
- Mga credential sa pag-access ng vault at lokal na key na protektado ng device-bound key para sa biometric access
- Mga preference sa seguridad tulad ng screenshot protection, clipboard clearing, biometric reauthentication, at awtomatikong proteksyon

Hindi ipinapadala sa developer ang iyong plaintext password. Isinasagawa ng operating system ang biometric authentication. Hindi nangongolekta ang app ng fingerprint o face images o biometric templates; natatanggap lamang nito ang resulta ng authentication.

### 2.3 Lokal na impormasyon sa aktibidad at backup

Maaaring lokal na mag-store ang app ng:

- Uri, paglalarawan, oras, at kaugnay na item identifiers para sa protection, locking, deletion, original deletion, backup, at restore events
- Hanggang 500 activity-log entries
- Backup destination, huling oras ng backup, bilang ng item, at status na tagumpay o pagkabigo
- Kung naka-enable ang automatic backup at ang password na kailangan upang i-update ang backup na iyon
- Mga pagpipilian sa ad privacy, restricted-data-processing choice, at bilang ng protected items na ginagamit para sa ad frequency

Ang sensitibong settings, kasama ang backup state at automatic-backup password, ay naka-store sa local store na naka-encrypt gamit ang device key. Responsibilidad mong panatilihing ligtas ang iyong backup password.

### 2.4 Impormasyong pinoproseso sa panahon ng advertising at consent

Sa suportadong advertising platform, kasalukuyang Android, maaaring gamitin ng app ang Google AdMob at UMP. Maaaring iproseso ng Google at advertising technology providers ang:

- Advertising, app-instance, o device-related identifiers
- IP address at tinatayang lokasyon na hinango mula sa impormasyon tulad ng IP address
- Device model, operating system, app version, wika, at network information
- Ad requests, impressions, clicks, interactions, at diagnostics
- Consent status at regional privacy choices

Maaaring gamitin ang impormasyong ito para sa ad delivery, non-personalized ads, frequency capping, measurement, fraud prevention, consent management, security, at legal compliance. Nakaka-implement ang app upang i-initialize ang Google Mobile Ads SDK lamang pagkatapos ipahiwatig ng UMP na maaaring humiling ng ads.

Tingnan ang [Google Privacy Policy](https://policies.google.com/privacy) at [impormasyon tungkol sa Google advertising technologies](https://policies.google.com/technologies/ads).

## 3. Mga layunin ng pagproseso

Pinoproseso ng FileGuard ang impormasyon upang:

- Mag-store at magpakita ng pinili o nakuhang content sa mga naka-encrypt na vault
- Kontrolin ang pag-access sa vault gamit ang locking, passwords, at biometric authentication
- Mag-import, mag-export, maglipat, mag-delete, at mag-track ng original-file status ng content
- Gumawa at mag-restore ng encrypted backups sa lokasyong pinili mo
- Panatilihin ang security preferences at linisin ang temporary decrypted files at clipboard contents
- Magpakita ng local security activity at error status
- Mag-deliver ng Android ads, kontrolin ang ad frequency, at magbigay ng privacy choices
- Pigilan ang abuse, protektahan ang service, at sumunod sa legal obligations

## 4. Storage at retention

| Kategorya | Storage at retention | Paano burahin |
|---|---|---|
| Encrypted vault files at metadata | Naka-store sa app-private local storage hanggang burahin mo | Burahin ang item o vault sa app, i-clear ang app data, o i-uninstall |
| Credentials at security settings | Naka-store sa operating-system secure storage at device-key-encrypted storage hanggang baguhin o alisin ang app data | I-disable ang kaugnay na feature, i-clear ang app data, o i-uninstall |
| Activity history | Hanggang 500 entries sa encrypted local storage | I-clear ang app data o i-uninstall |
| Temporary decrypted files | Pansamantalang isinusulat sa app cache at nililinis sa startup, backgrounding, o feature completion sa best-effort basis | Isara ang app o i-clear ang cache/data nito |
| Clipboard content | Pinoproseso sa pamamagitan ng operating-system clipboard kapag ginagamit ang copy o automatic protection | Automatic best-effort clearing, kumopya ng ibang content, o i-restart ang device |
| Encrypted backup files | Naka-store sa device folder, document provider, o cloud-synced location na pinili mo hanggang burahin mo | Burahin sa pamamagitan ng kaugnay na file manager o storage service |
| Google advertising data | Nire-retain ayon sa Google at processor policies at legal obligations | Baguhin ang app/device ad settings o gamitin ang Google privacy controls |

Maaaring magpanatili ang operating system, device manufacturer, document provider, o cloud backup provider ng hiwalay na kopya ng app data o backup files na ginawa mo. Ang mga kopyang iyon ay pinamamahalaan ng mga patakaran ng kaugnay na provider.

## 5. Third parties, service providers, at pagbebenta

Hindi ibinebenta ng developer ang vault content, passwords, o in-app activity history at hindi ibinibigay ang mga ito sa third parties sa pamamagitan ng server na pinapatakbo ng developer.

Kapag gumagana ang Android advertising o consent features, maaaring iproseso ng Google LLC, Google affiliates, advertising technology providers, at kaugnay na processors ang impormasyong inilalarawan sa Seksyon 2.4. Tingnan ang hiwalay na [International Data Transfer Notice](policy/).

Kung direkta kang pumili ng external app o cloud service sa pamamagitan ng file picker, sharing function, o backup destination, maaaring iproseso ng provider na iyon ang files ayon sa iyong direksyon. Nalalapat ang privacy policy at security settings nito, at hindi kinokontrol ng developer ang practices ng provider.

## 6. International data transfers

Hindi inililipat ang vault content sa server na pinapatakbo ng developer. Maaaring iproseso ng Google at kaugnay na processors ang advertising at consent information sa United States at iba pang bansa kung saan sila nagpapatakbo ng infrastructure.

Kung pumili ka ng overseas cloud service bilang lokasyon para sa encrypted backup, maaaring i-synchronize ang file sa servers sa labas ng iyong bansa ayon sa iyong direksyon. Tingnan ang [International Data Transfer Notice](policy/) para sa detalye.

## 7. Permissions

Maaaring gamitin ng app ang sumusunod na permissions o system capabilities kapag ginagamit mo ang kaugnay na feature:

- **Files and photos:** Mag-import lamang ng content na pinili mo
- **Camera:** Kumuha ng photos o videos para sa vault
- **Microphone:** Isama ang audio kapag nagre-record ng video
- **Biometrics:** Kumpirmahin ang vault access o sensitive settings changes
- **Internet at network state sa Android:** Humiling ng AdMob ads at UMP consent information
- **Advertising ID sa Android:** Suportahan ang Google advertising features
- **Clipboard:** Kumopya ng content o protektahan ang clipboard text kapag malinaw mong pinagana ang automatic protection

Ang pagtanggi sa permission ay maaaring mag-disable lamang ng kaugnay na feature. Kapag ginagamit ang system file picker, karaniwang limitado ang access sa mga item na pinili mo.

## 8. Security measures at limitations

Gumagamit ang kasalukuyang implementation ng mga hakbang na kinabibilangan ng:

- AES-256-GCM encryption para sa vault content at vault indexes
- PBKDF2-HMAC-SHA256 key derivation para sa password-based keys
- Android Keystore o StrongBox protection para sa local keys sa suportadong Android devices
- Device-key encryption para sa sensitive settings at activity history
- Best-effort vault locking at temporary-file at clipboard cleanup kapag pumapasok ang app sa background
- Optional screenshot protection at biometric reauthentication
- Password-encrypted portable backup packages

Walang security method na nag-aalis ng lahat ng panganib. Device theft, malware, operating-system vulnerabilities, mahihinang password, files na ibinahagi mo, o security issues sa external storage provider ay maaaring maglantad ng impormasyon.

Ang pagbukas o pag-export ng decrypted content sa ibang app ay maaaring gumawa ng hiwalay na kopya. Ang original-file deletion at temporary-file o clipboard cleanup ay maaaring malimitahan ng operating system, kaya dapat mong beripikahin ang pagtanggal ng sensitibong content.

## 9. Iyong mga karapatan at pagpipilian

Karamihan ng impormasyon ay nananatili lamang sa iyong device, kaya hindi ito maa-access, maitatama, o mabubura ng developer nang remote. Maaari mong:

- Burahin ang vault items o vaults sa app
- Baguhin ang security, biometric, automatic-protection, clipboard, at automatic-backup settings
- I-clear ang app data o cache, o i-uninstall ang app
- Burahin ang backup at exported files mula sa kanilang storage location
- Kung available, baguhin ang consent sa pamamagitan ng Google ad privacy options sa app
- Burahin o i-reset ang advertising identifier o limitahan ang ad personalization sa device settings

Maaari kang makipag-ugnayan sa amin tungkol sa impormasyong direkta mong ibinigay sa developer, tulad ng inquiry email. Kung naaangkop, maaaring bigyan ka ng lokal na batas ng mga karapatan sa access, correction, deletion, restriction, withdrawal of consent, at complaint sa supervisory authority.

## 10. Mga bata

Hindi pangunahing idinisenyo ang FileGuard para sa mga bata at hindi nito hinihingi sa mga bata na magbigay ng personal information. Maaaring gumamit ang guardians ng parental controls na ibinibigay ng device o app store. Ang under-age consent configuration para sa Android advertising ay dapat hiwalay na suriin laban sa intended audience at applicable law bago ang distribution.

## 11. Contact

Para sa mga tanong tungkol sa Patakarang ito:

- **Contact:** frog-im
- **Email:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

Para sa advertising data na pinoproseso ng Google, gamitin ang privacy controls at contact procedures na inilalarawan sa [Google Privacy Policy](https://policies.google.com/privacy).

## 12. Mga pagbabago sa Patakarang ito

Maaari naming i-update ang Patakarang ito kapag nagbago ang mga batas, app features, permissions, o third-party SDK practices. Ang material changes ay maaaring ipaalam sa pahinang ito, sa app, o sa distribution page.

Huling na-update: **Hunyo 23, 2026**
