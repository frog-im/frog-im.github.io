---
title: Politique de Confidentialité | TimeBack
description: Politique de confidentialité de TimeBack
lang: fr
last_updated: 2026-06-06
---

# Politique de confidentialité (TimeBack)

- **Nom de l'application :** TimeBack
- **Développeur :** frog-im
- **Contact :** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- **Date d'entrée en vigueur :** 2026-06-03
- **Dernière mise à jour :** 2026-06-06

Cette politique de confidentialité est basée sur la mise en œuvre actuelle de l'application TimeBack. TimeBack fournit une révision du temps d'écran, des objectifs quotidiens, des enregistrements de temps récupéré, des réflexions, des défis, des notifications, du partage et des fonctionnalités publicitaires.

## 1. Caractéristiques

TimeBack offre les fonctionnalités suivantes :

- Examen du temps d'utilisation de l'application via l'autorisation d'accès à l'utilisation d'Android
- Objectifs d'utilisation quotidiens, rappels et notifications d'utilisation dans la barre d'état
- Notifications d'avertissement de limite stricte et affichage en superposition
- Sélection d'applications d'exception de superposition
- Enregistrements d'activité de temps récupéré
- Enregistrements de réflexion quotidiens
- Progression du défi et gestion de la liste de contrôle
- Partage d'images avec statistiques d'utilisation
- Annonces Google AdMob et options de confidentialité basées sur UMP

## 2. Informations que nous traitons

### 2-1. Autorisation d'accès à l'utilisation en lecture des informations

Si l'utilisateur accorde l'autorisation à Android `PACKAGE_USAGE_STATS`, l'application peut lire les informations suivantes sur l'appareil :

- Nom du package d'application
- Nom de l'application
- Temps d'utilisation de l'application
- Plage de dates et d'heures utilisée pour l'agrégation de l'utilisation

Ces informations sont utilisées pour fournir des statistiques d'utilisation et comparer l'utilisation par rapport aux objectifs de l'utilisateur.

### 2-2. Informations saisies ou configurées par l'utilisateur

- Objectif d'utilisation quotidienne
- État et intervalle activés pour le rappel d'utilisation
- Paramètre d'affichage de l'utilisation de la barre d'état
- Catégorie d'activité de temps récupéré, titre, heure de début et durée
- Texte de réflexion quotidien
- Progression du défi et entrées de la liste de contrôle
- Liste des applications d'exception de superposition

### 2-3. Informations stockées sur l'appareil

L'application peut stocker les informations suivantes dans une base de données SQLite locale ou dans SharedPreferences :

- Enregistrements de temps d'utilisation de l'application
- Objectifs et paramètres quotidiens
- Enregistrements d'activité de temps récupéré
- Enregistrements de réflexion quotidiens
- Progression du défi et état de la liste de contrôle
- État d’achèvement de l’intégration
- Paramètres tels que les rappels d'utilisation, les avertissements de limite stricte, l'affichage de la barre d'état et les applications d'exception en superposition
- Consentement pour la publicité locale et état des options de confidentialité

Sur la base de la mise en œuvre actuelle, ces enregistrements locaux ne sont pas automatiquement téléchargés sur les serveurs frog-im.

### 2-4. Données de publicité et de consentement

Lorsque les annonces Google Mobile SDK (AdMob) et UMP sont utilisées, Google ou ses sociétés affiliées peuvent traiter des informations telles que :

- Identifiants publicitaires, tels qu'Android AD_ID
- Adresse IP et informations réseau
- Informations sur l'appareil, version OS et informations sur l'application
- Impressions publicitaires, clics, données de mesure et signaux d'erreur
- État du consentement à la publicité et des options de confidentialité
- Localisation approximative

## 3. Finalités du traitement

L'application traite les informations aux fins suivantes :

- Lire le temps d'utilisation, afficher des statistiques et comparer l'utilisation par rapport aux objectifs
- Stockage des enregistrements de temps récupéré et de réflexion saisis par l'utilisateur
- Gérer la progression des défis
- Fournir des rappels et des notifications dans la barre d'état
- Fournir des notifications d'avertissement de limite stricte, un affichage en superposition et une gestion des exceptions de superposition
- Partage d'images de statistiques d'utilisation à la demande de l'utilisateur
- Diffusion d'annonces, mesure des performances publicitaires et application des choix de consentement publicitaire
- Maintenir la stabilité de l'application et répondre aux erreurs

## 4. Stockage local et traitement externe

### 4-1. Stockage local

TimeBack stocke les données utilisateur principalement dans la mémoire interne de l'application sur l'appareil. Sur la base de la mise en œuvre actuelle, les enregistrements d'utilisation, les objectifs, les réflexions et les informations sur les défis ne sont pas automatiquement téléchargés sur les serveurs frog-im.

Le stockage local peut inclure les éléments suivants.

| Stockage | Articles stockés | But | Méthode de suppression |
|---|---|---|---|
| Base de données SQLite | Enregistrements d'utilisation des applications, noms de packages, noms d'applications, durée d'utilisation, agrégats basés sur la date | Afficher les statistiques d'utilisation et comparer l'utilisation par rapport aux objectifs | Fonctionnalités de suppression dans l'application, effacement des données de l'application ou désinstallation de l'application |
| Base de données SQLite | Activités de récupération, réflexions, progression du défi, entrées dans la liste de contrôle | Afficher les enregistrements et gérer les progrès | Fonctionnalités de suppression dans l'application, effacement des données de l'application ou désinstallation de l'application |
| Préférences partagées | État d'achèvement de l'intégration, paramètres de rappel, paramètres d'avertissement de limite stricte, paramètres d'affichage de la barre d'état, liste d'applications d'exception de superposition, état de consentement publicitaire local | Conserver les paramètres de l'application | Effacer les données de l'application ou désinstaller l'application |
| Fichiers/cache temporaires | Images de statistiques d'utilisation partagées et fichiers temporaires similaires | Effectuer le partage demandé par l'utilisateur | Supprimé après le partage lorsque cela est possible, ou conformément aux politiques de nettoyage de OS/app |

Lorsque l'utilisateur efface les données de l'application ou désinstalle l'application, les données stockées dans la mémoire interne de l'application sont généralement supprimées. Cependant, la sauvegarde Android, la sauvegarde du fabricant, la sauvegarde cloud ou les fichiers directement partagés par l'utilisateur peuvent être conservés séparément selon les politiques de ces services.

Les enregistrements d'utilisation et les textes de réflexion peuvent révéler des routines ou des intérêts personnels. Sur les appareils partagés, les utilisateurs doivent utiliser des mesures de protection appropriées telles que le verrouillage de l'appareil ou des comptes OS distincts.

### 4-2. Téléchargements sur le serveur

Sur la base du projet actuel, TimeBack ne télécharge pas automatiquement les enregistrements d'utilisation, les réflexions ou les enregistrements de défi sur les serveurs frog-im. Si l'utilisateur utilise la fonction de partage, une image statistique générée peut être transférée vers l'application ou le service externe sélectionné par l'utilisateur.

### 4-3. Traitement de la publicité

Google AdMob et UMP sont utilisés pour la publicité dans les applications et la gestion du consentement. Les informations liées à la publicité peuvent être traitées sur l'infrastructure de Google.

## 5. Services et processeurs tiers

### 5-1. Google AdMob/UMP

But:

- Diffusion de bannières publicitaires
- Gestion du consentement à la publicité et des options de confidentialité
- Mesure des performances publicitaires et prévention de la fraude

Informations susceptibles d'être traitées :

- Identifiants publicitaires
- Informations sur l'appareil et le réseau
- Informations sur les interactions avec les annonces
- État d’option de consentement et de confidentialité

### 5-2. Partage d'applications ou de services cibles

Si l'utilisateur utilise directement la fonctionnalité de partage d'images de statistiques d'utilisation, l'application ou le service externe sélectionné peut traiter l'image partagée. Ce traitement est régi par la politique de confidentialité du service sélectionné.

## 6. Avis de transfert transfrontalier

Les informations peuvent être traitées en dehors du pays de l'utilisateur dans les cas suivants.

| Article | Détails |
|---|---|
| Destinataire | Google LLC et ses sociétés affiliées |
| Destination | États-Unis et autres pays/régions où se trouve l'infrastructure Google |
| Timing | Lorsque l'application s'exécute, demande des publicités, affiche ou mesure des publicités, traite des clics ou gère le consentement |
| Méthode | Communication réseau cryptée (HTTPS/TLS) |
| But | Diffusion des annonces, gestion de l'état de personnalisation, mesure, analyse, amélioration de la stabilité du service, conformité légale |
| Données | Identifiants publicitaires, informations sur l'appareil/l'application/le réseau, informations sur les interactions publicitaires, état du consentement, emplacement approximatif, etc. |
| Rétention | Conformément aux politiques de Google et à la loi applicable |

Pour plus de détails, veuillez consulter le [Cross-Border Transfer Notice](./policy/).

## 7. Liste des applications installées et exceptions de superposition

Sur Android, si l'utilisateur configure des applications d'exception de superposition, l'application peut lire les noms de packages et les noms d'applications des applications pouvant être lancées sur l'appareil pour afficher une liste de sélection. Les noms de packages sélectionnés par l'utilisateur comme exceptions sont stockés dans SharedPreferences sur l'appareil et sont utilisés uniquement pour éviter d'afficher des superpositions d'avertissements de limites strictes au-dessus de ces applications.

## 8. Rétention

L'application conserve les informations selon les normes suivantes :

- Informations sur l'utilisation locale, les objectifs, la réflexion et les défis : jusqu'à ce que l'utilisateur les supprime, efface les données de l'application ou désinstalle l'application
- Paramètres SharedPreferences : jusqu'à ce que l'utilisateur efface les données de l'application ou désinstalle l'application
- Fichiers temporaires pour les images partagées : selon les besoins du partage ou conformément aux politiques de nettoyage OS
- Données relatives à la publicité et au consentement : conformément aux politiques de Google et d'autres tiers concernés

## 9. Autorisations

L'application peut utiliser les autorisations suivantes :

- `PACKAGE_USAGE_STATS` : lire la durée d'utilisation de l'application
- `POST_NOTIFICATIONS` : afficher les rappels d'utilisation et les notifications de la barre d'état
- `SYSTEM_ALERT_WINDOW` : afficher les superpositions d'avertissements de limites strictes
- `INTERNET` : communiquer avec les annonces SDK et afficher les pages de mentions légales
- `ACCESS_NETWORK_STATE` : vérifier l'état du réseau
- `com.google.android.gms.permission.AD_ID` : utiliser des identifiants publicitaires

Les autorisations sont utilisées uniquement si les fonctionnalités de l'application sont nécessaires. Les utilisateurs peuvent révoquer les autorisations dans les paramètres de l'appareil, mais les fonctionnalités associées peuvent être limitées.

## 10. Droits et choix des utilisateurs

Les utilisateurs peuvent :

- Afficher, modifier ou supprimer des enregistrements dans l'application
- Supprimez les informations locales en effaçant les données de l'application ou en désinstallant l'application
- Modifier les paramètres d'accès à l'utilisation, de notification et d'identifiant publicitaire dans les paramètres de l'appareil
- Révoquer l'autorisation de superposition et modifier les paramètres de l'application d'exception de superposition
- Modifier les options de confidentialité des annonces
- Contactez-nous pour toute question de confidentialité ou demande de suppression

E-mail de contact : [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

## 11. Mesures de sécurité

L'application applique ou peut appliquer les garanties suivantes :

- Communication externe basée sur HTTPS/TLS
- Traitement des données prioritairement local
- Demandes d'autorisation minimales nécessaires pour les fonctionnalités de l'application
- Application de l'état de consentement à la publicité

Les conditions de sécurité des appareils telles que le rootage, le jailbreak, les logiciels malveillants ou l'utilisation d'appareils partagés peuvent créer des risques supplémentaires.

## 12. Confidentialité des enfants

TimeBack n'est pas conçu principalement pour les enfants. Les paramètres liés à l'âge ou les politiques de plate-forme de Google Mobile Ads SDK et UMP peuvent s'appliquer pendant la publicité et le traitement du consentement.

## 13. Modifications

Cette politique peut être mise à jour en raison de changements dans la loi, la configuration des services tiers ou les fonctionnalités de l'application. Les changements importants seront notifiés via une notification dans l'application ou en mettant à jour cette page.

## 14. Contacter

- Développeur: frog-im
- Courriel : [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
