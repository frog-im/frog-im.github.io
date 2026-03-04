---
title: Politique de confidentialité | know_me
description: know_me (PeopleNote, Memory for People) Politique de confidentialité (Français)
---

# Politique de confidentialité (know_me / PeopleNote, Memory for People)

- **Nom de l'application :** know_me (PeopleNote, Memory for People)
- **Développeur :** frog-im
- **Responsable de la protection des données personnelles / Personne de contact :** frog-im
- **Contact :** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- **Date d'entrée en vigueur :** 2026-03-04
- **Dernière mise à jour :** 2026-03-04

> La présente Politique a été rédigée sur la base des informations traitées par l'application et de ses fonctionnalités associées.  
> Si des lois ou réglementations impératives s'appliquent dans un pays ou une région spécifique, ces lois ou réglementations peuvent prévaloir.

---

## 1. Objet et champ d'application

`know_me` est une application conçue pour aider les utilisateurs à enregistrer et à gérer des informations sur des personnes et, si nécessaire, à sauvegarder, restaurer et partager ces informations sous forme de fichiers PDF.

Ses principales fonctionnalités comprennent :

- Le stockage d'informations propres à chaque personne (telles que le nom, un texte d'identification, des notes, des traits de personnalité, le pays, le genre, les coordonnées, etc.)
- Le classement par dossiers, la recherche et les fonctions de fusion
- L'ajout de photos et la gestion de leurs descriptions
- L'exportation et l'importation de sauvegardes (`.knm`)
- L'exportation de fichiers PDF
- Le verrouillage de l'application (mot de passe/schéma)
- La gestion de la publicité et du consentement (AdMob/UMP)

L'application ne nécessite pas de création de compte distincte, et les données principales de l'utilisateur sont généralement stockées localement sur l'appareil de l'utilisateur.  
Toutefois, certains SDK tiers intégrés pour la gestion de la publicité et du consentement peuvent traiter certaines informations.

---

## 2. Catégories de données personnelles traitées

### 2-1) Informations saisies directement par l'utilisateur

Les informations suivantes ne sont stockées que lorsque l'utilisateur les saisit directement :

- Nom
- Texte d'identification (par exemple, apparence/caractéristiques utilisé comme texte de note)
- Notes
- Traits de personnalité, pays, genre
- Numéro de téléphone
- Texte relatif au moment d'apparition / au moment de la rencontre
- Informations sur la plateforme/le site
- Nom/couleur du dossier
- Description de l'image (caption)

### 2-2) Fichiers sélectionnés sur l'appareil

- Fichiers image sélectionnés par l'utilisateur lors de l'ajout de photos
- Fichiers de sauvegarde `.knm` sélectionnés par l'utilisateur lors de l'importation de sauvegardes
- Chemins d'enregistrement et fichiers enregistrés sélectionnés par l'utilisateur lors de l'exportation de PDF/sauvegardes

### 2-3) Données stockées localement dans l'application

Les données suivantes peuvent être stockées sur l'appareil de l'utilisateur afin de fournir les fonctionnalités de l'application :

- Base de données SQLite (`people_note.db`) : métadonnées relatives aux personnes/dossiers/plateformes/sites/images
- Fichiers image : chiffrés et stockés dans le dossier de documents de l'application (`.enc`)
- Paramètres de l'application (`SharedPreferences`) : thème, tri, options de confidentialité/publicité, options de masquage PDF, politiques de verrouillage de l'application, etc.
- Informations de verrouillage de l'application : valeurs de hachage et sels pour les mots de passe/schémas (`SharedPreferences`)
- Clés de chiffrement locales : stockées dans `flutter_secure_storage`
- Fichiers temporaires : aperçus de déchiffrement d'images, fichiers de cache d'import/export, etc. (dossier temporaire)

### 2-4) Informations pouvant être traitées automatiquement lors de la gestion de la publicité et du consentement

Lorsque les fonctionnalités de publicité ou de gestion du consentement sont activées, les SDK de Google LLC et de partenaires associés (tels qu'AdMob et UMP) peuvent traiter automatiquement les informations suivantes :

- Identifiants publicitaires (AAID/IDFA, etc.)
- Adresse IP et informations réseau
- Informations sur l'appareil (version du système d'exploitation, modèle de l'appareil, version de l'application, etc.)
- Informations relatives aux interactions avec les annonces (impressions, clics, etc.)
- Statut du consentement et informations sur les choix de confidentialité
- Informations liées au diagnostic, aux performances et à la sécurité

Les données principales de l'utilisateur de l'application ne sont généralement pas téléversées sur le serveur du développeur, mais une partie des informations ci-dessus peut être transmise à des services tiers pendant l'utilisation des fonctionnalités de publicité/consentement.

---

## 3. Finalités du traitement des données personnelles

L'application traite des données personnelles ou des informations associées aux fins suivantes :

- Enregistrer et consulter des informations sur des personnes, centrées sur les contacts/notes
- Fournir des fonctionnalités d'organisation, telles que le classement par dossiers, la recherche et la fusion
- Ajouter et afficher des photos
- Exécuter des fonctionnalités demandées par l'utilisateur, telles que la sauvegarde/restauration et l'exportation en PDF
- Fournir des fonctionnalités de sécurité de verrouillage de l'application
- Fournir de la publicité, gérer le consentement, prévenir les activités frauduleuses et respecter les obligations légales

---

## 4. Durée de conservation et de stockage des données personnelles

- Données internes de l'application (SQLite, paramètres locaux, images chiffrées) : conservées sur l'appareil de l'utilisateur jusqu'à la suppression de l'application, l'effacement des données de l'application ou la suppression directe des données par l'utilisateur
- Fichiers temporaires : supprimés après la fin de la tâche concernée ou effacés conformément à la politique de cache du système d'exploitation
- Fichiers exportés par l'utilisateur (PDF, fichiers de sauvegarde) : peuvent rester dans l'emplacement de stockage choisi par l'utilisateur et doivent être supprimés directement par l'utilisateur
- Données liées à la publicité/au consentement (traitées par des tiers) : soumises aux politiques de chaque prestataire de services et aux lois applicables

En principe, l'application ne stocke pas les données principales de l'utilisateur sur le serveur du développeur.  
Toutefois, les fichiers que l'utilisateur enregistre directement sur un stockage externe sont gérés dans l'environnement propre de l'utilisateur.

---

## 5. Procédures et méthodes de suppression des données personnelles

Lorsque la finalité du traitement est atteinte ou lorsque l'utilisateur demande la suppression, l'application supprime les informations concernées ou les traite de manière à ce qu'elles ne soient plus référencées, comme suit.

### 5-1) Procédures de suppression

- Lorsque l'utilisateur supprime directement des fiches individuelles de personnes, des dossiers, des images, des données de sauvegarde, etc., ces données sont considérées comme devant être supprimées immédiatement.
- Lorsque l'utilisateur supprime l'application ou efface les données de l'application depuis les paramètres de l'appareil, les données stockées dans la zone de stockage interne de l'application sont supprimées conformément aux procédures de suppression du système d'exploitation.
- Les fichiers temporaires font l'objet d'un nettoyage une fois la tâche concernée terminée, et certaines données mises en cache peuvent rester pendant un certain temps selon la politique du système d'exploitation.

### 5-2) Méthodes de suppression

- Données SQLite : suppression des enregistrements concernés
- Paramètres de l'application (`SharedPreferences`) : suppression de la clé concernée ou de l'ensemble des paramètres
- Valeurs de `flutter_secure_storage` : suppression des éléments de stockage sécurisé concernés
- Fichiers internes de l'application (images chiffrées, fichiers temporaires, etc.) : suppression des fichiers concernés
- PDF/fichiers de sauvegarde enregistrés directement par l'utilisateur sur un stockage externe : non supprimés automatiquement par l'application et devant être supprimés directement par l'utilisateur

Sauf obligation contraire prévue par la législation applicable, le développeur ne stocke pas séparément les données principales de l'utilisateur sur son serveur.

---

## 6. Communication à des tiers, sous-traitance et transfert international

L'application peut utiliser les services de Google pour la gestion de la publicité et du consentement.

| Élément | Détails |
|---|---|
| **Destinataire / Sous-traitant** | Google LLC et ses sociétés affiliées (exploitants d'AdMob/UMP) |
| **Pays de transfert** | États-Unis et régions où l'infrastructure de Google est exploitée |
| **Moment du transfert** | De manière continue lors des demandes d'annonces, des vérifications du statut du consentement, de l'initialisation du SDK et du fonctionnement |
| **Méthode de transfert** | Transmission via des communications réseau entre l'application et des serveurs tiers |
| **Base juridique du transfert international** | Traitement dans la mesure nécessaire à la fourniture du service sur la base de fondements juridiques applicables ou, si nécessaire, sur la base du consentement de la personne concernée |
| **Finalité** | Diffusion d'annonces, mesure publicitaire, gestion du consentement, prévention de la fraude et respect des politiques/lois |
| **Catégories de données (exemples)** | Identifiants publicitaires (AAID/IDFA), informations IP/réseau, informations sur l'appareil/l'application, informations relatives aux interactions avec les annonces, statut du consentement |
| **Durée de conservation** | Soumise aux politiques de Google et aux lois applicables |
| **Effet du refus** | Les annonces personnalisées peuvent être limitées, des annonces non personnalisées peuvent être affichées ou certaines fonctionnalités liées à la publicité peuvent être restreintes |

Le développeur ne collecte ni ne vend les données principales relatives aux fiches de personnes de l'application par l'intermédiaire de son propre serveur.

---

## 7. Informations sur les autorisations utilisées

L'application peut utiliser les autorisations suivantes :

- `INTERNET` : communication pour les SDK publicitaires et les fonctionnalités réseau associées
- `com.google.android.gms.permission.AD_ID` : utilisation des identifiants publicitaires (AdMob)
- `READ_MEDIA_IMAGES` (Android 13 et versions ultérieures), `READ_EXTERNAL_STORAGE` (Android 12 et versions antérieures) : ajout/sélection de photos

Les autorisations ne sont utilisées que dans la mesure nécessaire à la fourniture des fonctionnalités concernées.

---

## 8. Installation, fonctionnement et refus des mécanismes de collecte automatique

Cette application n'utilise pas directement des cookies généraux de sites web.  
Toutefois, dans le cadre des fonctionnalités de publicité et de gestion du consentement, des SDK tiers peuvent traiter automatiquement des identifiants publicitaires, des informations réseau, des informations sur l'appareil et des données similaires.

Les utilisateurs peuvent ajuster les paramètres concernés de la manière suivante :

- Modifier les choix dans les options de confidentialité ou l'écran de gestion du consentement de l'application (lorsqu'ils sont disponibles)
- Réinitialiser ou supprimer l'identifiant publicitaire dans les paramètres du système d'exploitation de l'appareil
- Limiter la publicité personnalisée ou ajuster les options de confidentialité associées dans les paramètres du système d'exploitation de l'appareil

Si l'utilisateur limite la publicité personnalisée, des annonces non personnalisées peuvent être affichées ou certaines fonctionnalités liées à la publicité peuvent être restreintes.

---

## 9. Droits des utilisateurs et modalités d'exercice

Sous réserve de la législation applicable, les utilisateurs peuvent disposer des droits suivants :

- Demander l'accès aux données personnelles, leur rectification ou leur suppression
- Demander la suspension ou la limitation du traitement
- Retirer le consentement pour les traitements fondés sur le consentement
- Modifier les choix en matière de publicité/consentement

Ces droits peuvent être exercés de la manière suivante :

- Modifier ou supprimer directement des données dans l'application
- Réinitialiser les données locales en supprimant les données de l'application ou en désinstallant l'application
- Modifier le consentement publicitaire via les options de confidentialité/l'écran de consentement de l'application (dans les régions où cette fonctionnalité est proposée)
- Réinitialiser/supprimer l'identifiant publicitaire ou limiter la publicité personnalisée via les paramètres du système d'exploitation de l'appareil
- Contact : [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

---

## 10. Mesures de sécurité

Le développeur applique ou s'efforce d'appliquer les mesures suivantes :

- Les données de l'utilisateur sont généralement stockées localement sur l'appareil
- Les fichiers image joints sont stockés localement sous forme chiffrée (basé sur AES-GCM)
- Les informations de verrouillage de l'application sont stockées sous forme de hachage plutôt qu'en texte brut
- Les fichiers de sauvegarde sont stockés après avoir été chiffrés sur la base d'un mot de passe utilisateur
- Les communications avec des SDK tiers sont chiffrées (HTTPS/TLS)
- Les autorisations sont utilisées avec une portée d'accès minimale

Toutefois, les risques résultant de l'état de sécurité de l'appareil de l'utilisateur (tels que le root/jailbreak, des applications malveillantes ou l'exposition d'un stockage partagé) ne peuvent pas être totalement éliminés.

---

## 11. Informations relatives aux données sensibles

Cette application n'exige pas la saisie de données sensibles.  
Il est conseillé aux utilisateurs de ne pas saisir de contenu sensible, tel que des informations de santé, des opinions politiques, une religion, des données biométriques ou des informations relatives à la vie sexuelle, dans les notes ou les champs de saisie libre.

Si un utilisateur saisit volontairement un contenu sensible, ces informations peuvent être stockées comme données locales sur l'appareil géré directement par l'utilisateur.

---

## 12. Protection des données personnelles des enfants

Cette application n'est pas conçue principalement pour les enfants.  
Les parents ou tuteurs peuvent gérer l'utilisation au moyen des fonctions de contrôle parental fournies par l'appareil ou la boutique d'applications.

---

## 13. Prise de décision automatisée

Cette application ne met pas en oeuvre de prise de décision automatisée fondée sur des données personnelles produisant des effets juridiques ou des effets significatifs similaires.

---

## 14. Avis relatif à la sécurité des données (Google Play, etc.)

Le développeur s'efforce de maintenir et de mettre à jour les éléments de divulgation relatifs à la sécurité des données dans les boutiques d'applications (telles que Google Play) conformément aux pratiques réelles de traitement de l'application et aux pratiques réelles de traitement des SDK tiers.

Toutefois, les informations affichées dans les boutiques d'applications peuvent varier en fonction de la version de l'application, du pays de distribution, de la configuration des SDK tiers et des changements de politique.

---

## 15. Avis relatif à l'open source

L'application utilise certaines bibliothèques open source.  
Les informations relatives aux licences correspondantes peuvent être consultées sur l'écran concerné dans l'application ou dans les avis fournis via le canal de distribution.

---

## 16. Contact

Pour toute question concernant la présente Politique de confidentialité :

- **Responsable de la protection des données personnelles / Personne de contact :** frog-im
- **E-mail :** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

---

## 17. Modifications de la présente Politique de confidentialité

La présente Politique peut être révisée en raison de modifications des lois/politiques, des fonctionnalités de l'application ou des SDK tiers.  
En cas de modifications substantielles, une notification peut être fournie au moyen d'avis dans l'application, sur la page de distribution ou via des mises à jour de la page de politique.

Dernière mise à jour : **2026-03-04**
