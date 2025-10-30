---
title: Politique de confidentialité | Lyrics Overlay & Tag Editor
description: Politique de confidentialité de Lyrics Overlay & Tag Editor (Français)
lang: fr
last_updated: 2025-10-30
---

# Politique de confidentialité (Lyrics Overlay & Tag Editor)

- **Nom de l’app :** Lyrics Overlay & Tag Editor  
- **Développeur :** frog-im  
- **Contact :** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com) 
- **Date d’entrée en vigueur :** 2025-10-30

> La présente Politique est rédigée en référence aux lois applicables, notamment la loi coréenne sur la protection des informations personnelles (PIPA), le RGPD/UK GDPR, la LPD suisse et les lois américaines des États en matière de vie privée. En cas d’exigences propres à une juridiction, ces exigences prévalent.

---

## 1. Finalité et champ d’application

Cette app fournit des fonctions **d’édition des métadonnées** (titre, artiste, etc.) des fichiers audio **stockés sur l’appareil**, ainsi qu’un **overlay de paroles**.  
L’app **ne** crée **aucun compte** et **n’envoie** pas les contenus de l’utilisateur vers des serveurs. Le traitement est effectué **par défaut sur l’appareil de l’utilisateur**.

Toutefois, à des fins **publicitaires** et de **conformité légale**, des partenaires tiers (p. ex. Google Mobile Ads SDK (AdMob), UMP) peuvent collecter et traiter des informations telles que des **identifiants publicitaires**. La collecte du consentement et les choix de confidentialité suivent les spécifications de la **User Messaging Platform (UMP) de Google**.

---

## 2. Catégories d’informations traitées

### 2-1) Fichiers explicitement sélectionnés par l’utilisateur
- **Chemins et contenus des fichiers audio/images de couverture :** traités **localement** sur l’appareil uniquement pour l’édition/l’enregistrement.  
- **FFmpegKit** est utilisé localement pour l’encodage, l’édition de métadonnées et l’extraction de miniatures.  
- L’app **n’upload** pas les fichiers sélectionnés par l’utilisateur vers nos serveurs.

### 2-2) Paramètres locaux et valeurs stockées

Pour le bon fonctionnement et le confort d’usage, l’app stocke les valeurs suivantes **localement sur l’appareil**.  
Ces valeurs ne sont pas envoyées à nos serveurs et **sont supprimées lors de la suppression des données de l’app ou de sa désinstallation**.

#### (1) Préférences (`shared_preferences`)
| Type | Clé/Contenu | Finalité | Emplacement | Suppression |
|---|---|---|---|---|
| Position/Police de l’overlay | `overlay_box_x`, `overlay_box_y`, `overlay_text_font` | Restaurer la position de l’overlay et la taille de police | SharedPreferences de l’appareil | Supprimé lors de l’effacement des données ou de la désinstallation |
| Publicité/Confidentialité | `pref_npa_always`, `pref_us_rdp`, `pref_child_directed`, `pref_under_age`, `pref_max_ad_rating` | Annonces non personnalisées, RDP (États-Unis), balise COPPA, balise d’âge, limite de classement du contenu publicitaire | SharedPreferences de l’appareil | Idem à gauche |

#### (2) Fichiers temporaires (dossier temporaire du système)
- **Exemples :** `cover_*.jpg`, `tmp_*.flac`  
- **Usage :** extraction de cover art, insertion de tags FLAC, encodages temporaires  
- **Emplacement :** dossier temporaire de l’OS (`systemTemp`)  
- **Rétention :** supprimés par l’app après traitement si possible ; le système peut également procéder à un nettoyage périodique

#### (3) Enregistrement choisi par l’utilisateur (SAF)
- Avec « Enregistrer sous », les fichiers finaux peuvent être écrits dans des emplacements choisis (p. ex. Téléchargements, cloud).  
- Ces fichiers résident dans la **mémoire externe** et **demeurent après la désinstallation**. L’utilisateur peut les supprimer manuellement.

#### (4) État du consentement (cache du SDK UMP)
- Dans l’EEE/Royaume-Uni/Suisse, le SDK UMP **met en cache localement** l’état du consentement publicitaire.  
- Réinitialisable via la suppression des données de l’app ou l’écran **Options de confidentialité** lorsqu’il est disponible.

---

### 2-3) Données publicitaires et de consentement (SDK tiers)
- **Google Mobile Ads SDK (AdMob) et UMP** peuvent collecter/traiter, par exemple : **identifiants publicitaires (AAID/IDFA)**, **plages d’IP**, **informations appareil/app**, **signaux d’interaction avec les annonces**, **état du consentement**, etc.  
- **Finalités :** diffusion d’annonces, limitation de fréquence, prévention de la fraude, mesure de performance, conformité légale  
- **Régions soumises au consentement (EEE/Royaume-Uni/Suisse) :** consentement recueilli via UMP ; **Options de confidentialité** fournies si nécessaire.  
  Dans les régions sans exigence correspondante (p. ex. KR), cette option **peut ne pas s’afficher**.

---

## 3. Traitement et durée de conservation

- **Paramètres locaux :** conservés sur l’appareil jusqu’à suppression des données de l’app ou désinstallation  
- **Fichiers temporaires :** créés lors de l’encodage/de l’extraction ; supprimés après traitement ou susceptibles de rester temporairement en cache  
- **Données publicitaires/de consentement (tiers) :** conformément aux **politiques de Google**

---

## 4. Fourniture à des tiers et transferts transfrontaliers

Pour la publicité et la gestion du consentement, des informations utilisateur peuvent être transmises à l’infrastructure de Google et y être traitées.

| Élément | Détails |
|---|---|
| **Destinataire** | Google LLC et ses affiliés/sous-traitants |
| **Destination** | États-Unis (et autres régions où se trouve l’infrastructure de Google) |
| **Finalité** | Diffusion d’annonces, performance/mesure, conformité légale, gestion du consentement |
| **Données** | Identifiants publicitaires, plages d’IP, infos appareil/app, interactions publicitaires, état du consentement, etc. |
| **Conservation** | Selon les politiques de Google |
| **Effet d’un refus** | Personnalisation limitée ; possibilité d’afficher uniquement des annonces non personnalisées |

Nous respectons les exigences de divulgation du module **« Sécurité des données » de Google Play** et maintenons ces divulgations conformes aux traitements réels.

---

## 5. Vos droits et leur exercice

- **Désactiver les annonces personnalisées / modifier le consentement**  
  - Dans les régions prises en charge (EEE/Royaume-Uni/Suisse) : ajustez dans **Réglages → Options de confidentialité**.  
  - Autres régions : utilisez les réglages de l’OS pour **réinitialiser l’ID publicitaire / limiter le suivi**.
- **Réinitialiser les informations locales :** la suppression des données de l’app ou sa désinstallation réinitialise les coordonnées d’overlay, la taille de police et autres réglages.
- Les droits prévus par le **RGPD/UK GDPR/LPD suisse/lois américaines des États** (accès, rectification, effacement, portabilité, limitation, retrait du consentement, etc.) peuvent être exercés selon les procédures prévues.  
  Pour les données publicitaires traitées par Google, veuillez utiliser les **procédures de Google**.

---

## 6. Données des enfants

Cette app **n’est pas destinée aux enfants**. Un enfant en-dessous de l’âge légal minimal doit cesser l’utilisation et recourir, avec son responsable légal, aux fonctions de limitation publicitaire au niveau de l’OS. Le cas échéant, nous pouvons appliquer **TFUA (balise « destiné aux enfants »)** ou des options équivalentes.

---

## 7. Mesures de sécurité

- **Minimisation des données** lors de la collecte et du stockage  
- **Usage limité** des fichiers temporaires et suppression après traitement lorsque possible  
- Traitement **dans le périmètre des autorisations OS**  
- **Chiffrement en transit** (TLS ou équivalent) pour les transferts tiers conformément aux standards des SDK

---

## 8. Sécurité des données (Google Play)

Nous préparons et tenons à jour de manière exacte la section **« Sécurité des données »** dans la Play Console, et la mettons à jour sans délai en cas de changements.

---

## 9. Mentions open source

L’app utilise des logiciels open source tels que **FFmpeg**. Un fichier d’information (p. ex. `open-source/ffmpeg/WHERE-TO-GET-SOURCE.txt`) inclus dans l’app explique comment obtenir le code source. Sur demande, nous le fournirons conformément à ce fichier.

---

## 10. Contact

- E-mail : [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

---

## 11. Modifications de la présente Politique

Nous pouvons réviser cette Politique en raison d’évolutions légales ou de service. Les changements seront publiés **dans l’app** et sur cette **page de politique**.  
En cas de modifications importantes, un préavis sera donné **au moins 7 jours avant** la date d’effet.

---

## Annexe : Guide utilisateur

- **Lien in-app :** ouvrir cette page via **Réglages → Confidentialité**.  
- **Comportement régional :** dans l’EEE/Royaume-Uni/Suisse, les Options de confidentialité sont affichées. **En KR et dans certaines autres régions, le bouton peut ne pas afficher d’options supplémentaires** lorsqu’aucune obligation légale ne l’exige.


