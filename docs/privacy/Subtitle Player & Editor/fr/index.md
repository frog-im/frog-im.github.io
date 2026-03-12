---
title: Politique de confidentialité | Subtitle Tool
description: Politique de confidentialité de Subtitle Tool (Subtitle Player & Editor) - Français
lang: fr
last_updated: 2026-03-11
---

# Politique de confidentialité (Subtitle Tool / Subtitle Player & Editor)

- **Nom de l’application :** Subtitle Player & Editor (également désigné comme **Subtitle Tool** dans la présente Politique)
- **Développeur :** frog-im
- **Contact :** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- **Date d’entrée en vigueur :** 2026-03-11

> Cette Politique est préparée en référence aux lois applicables, notamment la loi coréenne sur la protection des informations personnelles (PIPA), le RGPD / UK GDPR, la LPD suisse, ainsi que les lois pertinentes des États américains en matière de confidentialité. Si des règles locales obligatoires s’appliquent, ces règles prévalent.

---

## 1. Objet et portée

Cette application fournit :

- la lecture et l’édition de sous-titres
- la lecture vidéo + sous-titres à partir de fichiers sélectionnés par l’utilisateur
- une superposition flottante de sous-titres / paroles affichée au-dessus d’autres applications sur Android

La gestion des sous-titres prise en charge peut inclure des formats tels que :

- `srt`
- `vtt`
- `ass`
- `ssa`
- `lrc`
- `txt`

L’application ne crée **pas** de compte utilisateur et ne téléverse **pas** les fichiers de sous-titres ou de médias de l’utilisateur vers les propres serveurs du développeur. L’analyse, l’édition, l’aperçu des sous-titres et la plupart des traitements liés à la lecture sont effectués **localement sur l’appareil**.

Cependant, à des fins de publicité, de gestion du consentement et de conformité légale, des SDK tiers tels que **Google Mobile Ads SDK (AdMob)** et **Google UMP** peuvent traiter certaines informations, telles que les identifiants publicitaires, les signaux de l’appareil et les choix de consentement.

---

## 2. Catégories d’informations que nous traitons

### 2-1) Fichiers explicitement choisis par l’utilisateur

L’application interagit avec les fichiers explicitement sélectionnés par l’utilisateur, notamment :

- **Fichiers de sous-titres**
  - Exemples : `.srt`, `.vtt`, `.ass`, `.ssa`, `.lrc`, `.txt`
  - Utilisations :
    - lecture des sous-titres dans l’application
    - édition des sous-titres
    - affichage des sous-titres en superposition
    - conversion et exportation des sous-titres

- **Fichiers multimédias**
  - Exemples : fichiers vidéo ou audio locaux choisis par l’utilisateur
  - Utilisations :
    - lecture vidéo + sous-titres
    - alignement temporel de la superposition avec le média en cours de lecture

Points importants :

- Les fichiers sélectionnés par l’utilisateur sont traités localement sur l’appareil.
- L’application ne téléverse pas ces fichiers vers les propres serveurs du développeur.
- Les chemins et contenus des fichiers sont utilisés uniquement pour la lecture, la superposition, l’édition, l’enregistrement et les actions demandées par l’utilisateur.

### 2-2) Paramètres locaux et valeurs stockées

Afin de fournir des paramètres persistants et de restaurer l’état antérieur, l’application stocke certaines valeurs localement sur l’appareil à l’aide de `SharedPreferences` ou d’un stockage local similaire fourni par le système d’exploitation.

Ces valeurs ne sont pas envoyées vers les propres serveurs du développeur et sont normalement supprimées si les données de l’application sont effacées ou si l’application est désinstallée.

#### (1) Paramètres de superposition

Exemples :

- `overlay_box_x`
- `overlay_box_y`
- `overlay_text_font`
- `overlay_text_color`
- `overlay_outline_enabled`
- `overlay_outline_color`
- `overlay_outline_width`
- `overlay_force_landscape`
- `overlay_interstitial_count`

Finalité :

- restaurer la position de la superposition
- restaurer le style des sous-titres pour la superposition et la lecture des sous-titres dans l’application
- conserver les préférences de contour / police / orientation
- contrôler la logique de fréquence d’affichage des publicités dans certains flux liés à la superposition

#### (2) Positions récentes de lecture ou de superposition

Exemples :

- `overlay_recent_positions`
- `video_subtitle_recent_position`

Finalité :

- restaurer ou suggérer les positions de départ récentes pour les sous-titres/la superposition
- reprendre plus facilement la lecture vidéo + sous-titres

#### (3) Valeurs de préférences publicitaires et de confidentialité

Exemples possibles :

- `pref_npa_always`
- `pref_us_rdp`
- `pref_child_directed`
- `pref_under_age`
- `pref_max_ad_rating`

Finalité :

- stocker les choix de confidentialité liés à la publicité
- appliquer les paramètres de confidentialité et de configuration publicitaire de UMP / AdMob

#### (4) Fichiers de sous-titres créés par l’utilisateur

Lorsque l’utilisateur enregistre ou exporte des fichiers de sous-titres, l’application peut écrire de nouveaux fichiers de sous-titres à un emplacement sélectionné par l’utilisateur, tel que :

- Téléchargements
- un autre dossier sélectionné via un sélecteur système
- un emplacement de stockage géré par l’utilisateur

Ces fichiers enregistrés par l’utilisateur peuvent rester sur l’appareil après la suppression de l’application, sauf si l’utilisateur les supprime manuellement.

#### (5) Fichiers temporaires et caches

L’application et des bibliothèques tierces peuvent créer des fichiers temporaires ou de cache pour le fonctionnement normal, tels que :

- données de cache du sélecteur de fichiers
- données temporaires de conversion de sous-titres
- données de cache liées à la lecture

Ils sont destinés uniquement au fonctionnement local et ne sont pas téléversés vers les propres serveurs du développeur.

#### (6) Cache de l’état de consentement UMP

Dans les régions où Google UMP s’applique, le SDK peut mettre en cache localement sur l’appareil l’état du consentement.

Cela peut généralement être réinitialisé en :

- effaçant les données de l’application, ou
- modifiant les choix de consentement dans l’application lorsqu’une entrée relative aux options de confidentialité est disponible

### 2-3) Traitement lié à la superposition Android et aux autorisations

Sur Android, la superposition flottante de sous-titres peut utiliser :

- l’autorisation `SYSTEM_ALERT_WINDOW` / affichage au-dessus des autres applications
- l’autorisation `POST_NOTIFICATIONS`
- une notification de service en premier plan requise pour le service de superposition

Finalité :

- afficher la superposition de sous-titres au-dessus d’autres applications
- maintenir le service de superposition en fonctionnement
- permettre à Android d’afficher les notifications requises pour la superposition / le service
- lire les informations des notifications multimédias lorsque cela est nécessaire pour la prise en charge de la progression des sous-titres

Ces autorisations sont utilisées uniquement pour les fonctionnalités de l’application que l’utilisateur choisit d’utiliser.

### 2-4) Publicités, consentement et données associées (SDK tiers)

L’application utilise des SDK Google de publicité / consentement, notamment :

- **Google Mobile Ads SDK (AdMob)**
- **Google UMP**

L’application peut afficher :

- des bannières publicitaires
- des publicités interstitielles
- des publicités avec récompense ou interstitielles avec récompense

Ces SDK peuvent traiter des données telles que :

- des identifiants publicitaires (par exemple, AAID / IDFA le cas échéant)
- des informations liées à l’adresse IP et au réseau
- des métadonnées sur l’appareil et l’application
- des signaux d’interaction avec les publicités
- des choix de consentement

Les finalités peuvent inclure :

- la diffusion de publicités
- la mesure et les rapports publicitaires
- la limitation de fréquence
- la prévention de la fraude
- la conformité légale

Le développeur s’efforce de configurer ces SDK d’une manière conforme aux choix de consentement de l’utilisateur et au droit applicable.

---

## 3. Comment nous traitons et conservons les données

- **Paramètres locaux et données de position récente**
  - conservés sur l’appareil jusqu’à ce que les données de l’application soient effacées ou que l’application soit supprimée

- **Fichiers temporaires / cache**
  - conservés uniquement aussi longtemps que nécessaire au fonctionnement, puis supprimés par l’application lorsque cela est possible en pratique, ou nettoyés ultérieurement par le système d’exploitation

- **Fichiers de sous-titres enregistrés par l’utilisateur**
  - restent dans l’emplacement de sauvegarde choisi par l’utilisateur jusqu’à leur suppression par celui-ci

- **Données publicitaires / de consentement traitées par des tiers**
  - conservées conformément aux politiques de Google et au droit applicable

---

## 4. Traitement par des tiers et transferts transfrontaliers

Pour la publicité et la gestion du consentement, certaines informations peuvent être traitées par Google et des partenaires associés.

| Élément | Détails |
|---|---|
| Destinataire | Google LLC et sociétés affiliées / sous-traitants concernés |
| Finalité | Diffusion de publicités, mesure, prévention de la fraude, gestion du consentement et conformité légale |
| Données possibles | Identifiants publicitaires, informations sur l’appareil/l’application, informations fondées sur l’IP, données d’interaction publicitaire, état du consentement |
| Destination | États-Unis et autres régions où l’infrastructure de Google opère |
| Conservation | Conformément aux politiques de Google et au droit applicable |

Le développeur s’efforce de maintenir des informations de confidentialité cohérentes dans les stores d’applications avec le comportement réel des SDK.

---

## 5. Vos droits et vos choix

Selon votre juridiction, vous pouvez disposer de droits tels que :

- accès
- rectification
- suppression
- limitation
- portabilité
- opposition
- retrait du consentement lorsque le consentement constitue la base légale

Les moyens de contrôle pratiques comprennent :

- la modification des choix relatifs à la publicité / à la confidentialité dans l’application lorsque cette possibilité existe
- l’effacement des données de l’application pour supprimer les paramètres locaux et les préférences mises en cache
- la désinstallation de l’application
- la suppression manuelle des fichiers de sous-titres exportés depuis le stockage de l’utilisateur
- l’utilisation des contrôles au niveau du système d’exploitation, tels que les paramètres de notification, la réinitialisation de l’identifiant publicitaire ou les paramètres de personnalisation des publicités

Pour les données traitées par Google, les utilisateurs doivent également consulter les propres outils de confidentialité et de compte de Google, le cas échéant.

---

## 6. Confidentialité des enfants

Cette application n’est pas principalement destinée aux enfants.

Son objectif principal est la lecture, l’édition et l’affichage en superposition de sous-titres, ainsi que des fonctions utilitaires associées. Le cas échéant, la configuration des SDK publicitaires peut appliquer des indicateurs liés à l’âge ou destinés aux enfants, conformément aux exigences de la plateforme et aux paramètres du développeur.

---

## 7. Mesures de sécurité

Dans les limites de l’architecture de l’application, le développeur cherche à :

- minimiser la collecte en conservant la majorité du traitement des sous-titres et des médias sur l’appareil
- utiliser les sélecteurs de fichiers du système et l’accès aux fichiers initié par l’utilisateur
- utiliser les autorisations système de manière transparente
- s’appuyer sur le transport réseau chiffré utilisé par les SDK tiers, lorsque cela est applicable

Aucune méthode de stockage ou de transmission n’est parfaitement sûre, mais l’application est conçue pour éviter toute collecte inutile par le développeur.

---

## 8. Logiciels open source

L’application utilise des logiciels open source, y compris des bibliothèques liées à :

- l’analyse et la sérialisation des sous-titres
- la sélection de fichiers
- les préférences locales
- les fenêtres de superposition
- la lecture vidéo
- WebView

Les avis relatifs aux logiciels open source sont disponibles dans l’application. Pour certains composants, l’application peut utiliser une copie localement modifiée d’un paquet open source tout en conservant la mention de licence d’origine.

---

## 9. Contact

Si vous avez des questions ou des demandes liées à la confidentialité :

- **E-mail :** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

Veuillez inclure le nom de l’application **Subtitle Player & Editor** dans votre message.

---

## 10. Modifications de cette Politique

Cette Politique peut être mise à jour si :

- les fonctionnalités de l’application changent
- les autorisations ou l’utilisation des SDK changent
- les exigences légales ou de plateforme changent

Les modifications importantes seront reflétées dans la page de politique mise à jour et, le cas échéant, dans l’application.
