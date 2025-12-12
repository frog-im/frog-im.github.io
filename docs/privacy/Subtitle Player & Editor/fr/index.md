---
title: Politique de Confidentialité | Subtitle Tool
description: Politique de confidentialité de Subtitle Player & Editor (Subtitle Tool)
lang: fr
last_updated: 2025-12-12
---

# Politique de Confidentialité (Subtitle Player & Editor / « Subtitle Tool »)

- **Nom de l’application :** Subtitle Player & Editor (ci-après « Subtitle Tool »)  
- **Développeur :** frog-im  
- **Contact :** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)  
- **Date d’entrée en vigueur :** 2025-12-12  

> La présente Politique est rédigée en référence aux lois applicables, notamment la Loi coréenne sur la protection des informations personnelles (PIPA), le RGPD / RGPD du Royaume-Uni, la loi suisse FADP et diverses lois américaines relatives à la vie privée.  
> En cas de divergence, les exigences spécifiques à une juridiction donnée prévalent.

---

## 1. Objet et Champ d’Application

Cette application propose des fonctions d’**édition des métadonnées de fichiers audio** (titre, artiste, etc.) stockés sur l’appareil ainsi qu’une fonction de **superposition de paroles / sous-titres**.  
L’application **ne crée pas de compte utilisateur** et **ne téléverse pas** le contenu de l’utilisateur vers nos serveurs. Le traitement s’effectue **localement sur l’appareil** par défaut.

Cependant, à des fins de **publicité** et de **conformité légale**, des partenaires tiers (par exemple Google Mobile Ads SDK (AdMob) et UMP) peuvent collecter et traiter des informations telles que des **identifiants publicitaires**.  
La collecte du consentement et les choix de confidentialité suivent les spécifications de **Google UMP (User Messaging Platform)**.

---

## 2. Catégories d’Informations que Nous Traitions

### 2-1) Fichiers explicitement sélectionnés par l’utilisateur

- **Chemins et contenus audio / images de couverture :** traités **localement** sur l’appareil uniquement pour l’édition et l’enregistrement.  
- **FFmpegKit** est utilisé localement pour l’encodage, l’édition de métadonnées et l’extraction de vignettes.  
- L’application **ne téléverse pas** ces fichiers sélectionnés par l’utilisateur vers nos serveurs.

### 2-2) Paramètres locaux et valeurs stockées

Pour le bon fonctionnement et le confort d’utilisation, l’application enregistre les valeurs suivantes **localement sur l’appareil**.  
Ces données ne sont pas transmises à nos serveurs et sont **supprimées lorsque l’application ou ses données sont supprimées**.

#### (1) Préférences (`shared_preferences`)

| Type | Clé / Contenu | Finalité | Stockage | Suppression |
|---|---|---|---|---|
| Position / police de superposition | `overlay_box_x`, `overlay_box_y`, `overlay_text_font` | Restaurer la position de la superposition et la taille de police | SharedPreferences de l’appareil | Supprimées lors de l’effacement des données de l’app ou de sa désinstallation |
| Paramètres pub / confidentialité | `pref_npa_always`, `pref_us_rdp`, `pref_child_directed`, `pref_under_age`, `pref_max_ad_rating` | Annonces non personnalisées, signal U.S. RDP, balise COPPA, balise d’âge, limitation de la classification des contenus publicitaires | SharedPreferences de l’appareil | Idem ci-contre |

#### (2) Fichiers temporaires (dossier temporaire du système)

- **Exemples :** `cover_*.jpg`, `tmp_*.flac`  
- **Usage :** extraction de jaquettes, étiquetage FLAC, encodage temporaire  
- **Emplacement :** dossier temporaire du système (`systemTemp`)  
- **Durée de conservation :** supprimés par l’application après traitement lorsque cela est possible ; peuvent également être supprimés par les mécanismes de nettoyage du système.

#### (3) Enregistrements choisis par l’utilisateur (SAF)

- Lorsqu’un utilisateur choisit « Enregistrer sous », les fichiers audio finaux peuvent être écrits dans des emplacements désignés par l’utilisateur (par exemple Téléchargements, stockage cloud).  
- Ces fichiers résident dans le **stockage externe** et **peuvent subsister après la désinstallation**. L’utilisateur peut les supprimer manuellement.

#### (4) État du consentement (cache UMP)

- Dans les régions EEE / Royaume-Uni / Suisse, le SDK UMP **met en cache localement l’état du consentement publicitaire** de l’utilisateur.  
- Il peut être réinitialisé en supprimant les données de l’application ou via l’écran **Options de confidentialité** lorsque celui-ci est disponible.

---

### 2-3) Données liées aux annonces et au consentement (SDK tiers)

- **Google Mobile Ads SDK (AdMob) et UMP** peuvent collecter et traiter, par exemple : **identifiants publicitaires (AAID/IDFA)**, **plages d’IP**, **informations sur l’appareil / l’application**, **signaux d’interaction avec les annonces**, **état du consentement**, etc.  
- **Finalités :** diffusion d’annonces, limitation de fréquence, prévention de la fraude, mesure de performance, respect des obligations légales.  
- **Régions nécessitant un consentement (EEE / Royaume-Uni / Suisse) :** le consentement est recueilli via des écrans UMP, et un écran **Options de confidentialité** est fourni lorsqu’il est requis.  
  Dans d’autres régions (par ex. Corée), cette option **peut ne pas apparaître**.

---

## 3. Traitement et Durée de Conservation

- **Paramètres locaux :** conservés sur l’appareil jusqu’à ce que l’utilisateur supprime les données ou désinstalle l’application.  
- **Fichiers temporaires :** créés lors de l’encodage / extraction, puis supprimés après traitement ; peuvent rester de manière temporaire dans les caches système.  
- **Données d’annonces / de consentement (tiers) :** conservées et supprimées conformément aux **politiques de Google**.

---

## 4. Transferts à des Tiers et Flux Transfrontaliers

Pour la publicité et la gestion du consentement, certaines informations utilisateur peuvent être transmises à l’infrastructure de Google et y être traitées.

| Élément | Détails |
|---|---|
| **Destinataire** | Google LLC et ses filiales / sous-traitants |
| **Destination** | États-Unis (et autres régions où l’infrastructure de Google est hébergée) |
| **Finalité** | Diffusion d’annonces, mesure et performance, conformité légale, gestion du consentement |
| **Données** | Identifiants publicitaires, plages d’IP, infos appareil / app, interactions avec les annonces, état du consentement, etc. |
| **Durée de conservation** | Conformément aux politiques de Google |
| **Effet d’un refus** | Les annonces personnalisées peuvent être limitées ; des annonces non personnalisées peuvent être affichées |

Nous respectons les exigences de la section **« Sécurité des données » de Google Play** et alignons ces déclarations sur les traitements réels.

---

## 5. Vos Droits et la Manière de les Exercer

- **Désactivation des annonces personnalisées / modification du consentement**  
  - Dans les régions concernées (EEE / Royaume-Uni / Suisse) : modifiez vos préférences dans **Paramètres → Options de confidentialité**.  
  - Dans les autres régions : utilisez les paramètres du système d’exploitation pour **réinitialiser les identifiants publicitaires / limiter le suivi publicitaire**.
- **Réinitialisation des informations locales :** la suppression des données de l’application ou sa désinstallation réinitialise les coordonnées de superposition, la taille de police et les autres paramètres locaux.  
- Les droits conférés par le **RGPD / RGPD du Royaume-Uni / FADP suisse / lois américaines sur la vie privée** (accès, rectification, effacement, portabilité, limitation, retrait du consentement, etc.) peuvent être exercés dans la mesure prévue par ces lois.  
  Pour les données publicitaires traitées par Google, veuillez utiliser les **procédures mises en place par Google**.

---

## 6. Protection des Enfants

Cette application **n’est pas destinée aux enfants**.  
Si un enfant en dessous de l’âge minimum légal utilise l’application, il doit cesser de l’utiliser et recourir, avec son représentant légal, aux fonctions de limitation de la publicité offertes par le système d’exploitation.  
Le cas échéant, nous pouvons appliquer des balises telles que **TFUA (balise « child-directed »)** ou des options similaires de protection des enfants.

---

## 7. Mesures de Sécurité

- **Minimisation des données** collectées et stockées  
- Utilisation limitée de fichiers temporaires et suppression après traitement lorsque cela est possible  
- Traitement strictement **dans le cadre des autorisations du système d’exploitation**  
- Chiffrement **TLS ou équivalent** pour les transmissions à des tiers (conformément aux standards des SDK tiers)

---

## 8. Sécurité des Données (Google Play)

Nous préparons et maintenons de manière exacte la section **« Sécurité des données »** dans la Play Console, et nous la mettons à jour rapidement en cas de changement.

---

## 9. Mentions Relatives aux Logiciels Open Source

L’application utilise des logiciels open source tels que **FFmpeg**.  
Un fichier d’information (par exemple `open-source/ffmpeg/WHERE-TO-GET-SOURCE.txt`) au sein de l’application explique comment obtenir le code source.  
Sur demande, nous fournirons le code source conformément aux indications de ce fichier.

---

## 10. Contact

- E-mail : [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

---

## 11. Modifications de la Présente Politique

Nous pouvons réviser la présente Politique en raison de changements légaux ou de service.  
Les mises à jour seront publiées **dans l’application** et sur cette **page de politique**.  
En cas de changement important, un préavis sera fourni **au moins 7 jours avant** la date d’entrée en vigueur.
