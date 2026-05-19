---
title: Politique de confidentialité | QDiary
description: Politique de confidentialité de QDiary
---

# Politique de confidentialité (QDiary)

- Nom de l’application : QDiary
- Développeur : frog-im
- Contact : [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- Date d’entrée en vigueur : 2026-04-19
- Dernière mise à jour : 2026-04-19

La présente Politique de confidentialité est rédigée sur la base de l’implémentation actuelle de l’application QDiary. QDiary propose des fonctionnalités d’écriture de journal, de génération et de réflexion de quêtes, de connexion, de sauvegarde manuelle dans le cloud, de publicité et de notifications. Dans ce cadre, elle peut traiter des données à caractère personnel ou des informations pouvant constituer de telles données, dans la mesure nécessaire.

## 1. Fonctionnalités fournies

QDiary fournit les fonctionnalités suivantes :

- Rédaction, modification et consultation de journaux
- Classement par catégories et consultation via calendrier
- Génération de quêtes, réflexion sur les quêtes et gestion de l’achèvement des quêtes
- Verrouillage local de l’application de journal et chiffrement local
- Connexion par e-mail, vérification de l’adresse e-mail, connexion anonyme (invité) et réinitialisation du mot de passe
- Sauvegarde et chargement dans le cloud initiés par l’utilisateur
- Affichage de publicités et gestion des options de confidentialité liées aux publicités
- Notifications de rappel de quête

## 2. Catégories de données traitées

### 2-1. Informations saisies directement par l’utilisateur

- Adresse e-mail
- Mot de passe
- Titre, contenu, date, catégorie et niveau de difficulté du journal
- Réponses aux quêtes, contenu des réflexions et informations sur la quête sélectionnée
- Valeurs sélectionnées liées au profil de quête et texte de synthèse
- Phrase secrète pour le verrouillage de l’application de journal

### 2-2. Informations stockées par l’application sur l’appareil

- Base de données locale du journal (SQLite)
- Informations relatives à l’état des quêtes des journaux locaux
- Valeurs d’état liées à l’assiduité, aux paramètres, à la langue, aux notifications et aux publicités
- Valeurs de vérification du verrouillage de l’application, salt et métadonnées de chiffrement
- Informations de planification des notifications de quête

### 2-3. Informations relatives au compte et à l’identification

Les informations suivantes peuvent être traitées via Firebase Authentication :

- UID Firebase
- Adresse e-mail
- Indication de vérification de l’adresse e-mail
- Indication d’utilisation de la connexion anonyme

### 2-4. Informations relatives à la publicité et au consentement

Lors de l’utilisation de Google AdMob et du SDK UMP, les informations suivantes peuvent être traitées :

- Identifiants publicitaires (tels que Android AD_ID)
- Adresse IP et informations réseau
- Informations sur l’appareil, version du système d’exploitation et informations sur l’application
- Informations sur les impressions publicitaires, les clics et le traitement des récompenses
- Statut du consentement publicitaire et statut des options de confidentialité

### 2-5. Informations relatives aux notifications

- Indication de l’autorisation des notifications
- Valeurs d’identification des journaux contenant des quêtes en cours
- Texte des notifications de quête
- Horaires des notifications programmées

## 3. Finalités du traitement

L’application traite les informations pour les finalités suivantes :

- Inscription, connexion, vérification de l’adresse e-mail et réinitialisation du mot de passe
- Rédaction, sauvegarde et consultation des journaux
- Génération de quêtes, réflexion et détermination de l’achèvement
- Chiffrement et déchiffrement locaux liés au verrouillage de l’application
- Sauvegarde et chargement dans le cloud demandés par l’utilisateur
- Fourniture de notifications de quête
- Fourniture de publicités, traitement des récompenses publicitaires et prise en compte du statut de consentement publicitaire
- Sécurité, gestion des erreurs et exploitation du service

## 4. Stockage local, stockage dans le cloud et traitement externe

### 4-1. Stockage local

Les informations du journal et des quêtes sont principalement stockées dans la base de données locale de l’appareil.

- Si le verrouillage de l’application n’est pas activé : stockage local sous forme générale
- Si le verrouillage de l’application est activé : certaines informations, telles que le titre du journal, son contenu et l’état des quêtes, peuvent être chiffrées et stockées localement

### 4-2. Stockage dans le cloud

L’application stocke des données dans Firebase Firestore uniquement lorsque l’utilisateur exécute directement la fonction `Save`.

Selon la configuration actuelle du projet :

- Aucune synchronisation automatique complète n’est utilisée
- Les données ne sont stockées dans Firestore `savedDiaries` que lorsque l’utilisateur les enregistre manuellement
- Lors de l’enregistrement, le titre du journal, son contenu et l’état des quêtes peuvent être stockés sous forme chiffrée selon l’état actuel du verrouillage de l’application
- Les données ne sont rechargées dans le stockage local que lorsque l’utilisateur exécute `Load`

### 4-3. Traitement externe pour la génération et la réflexion sur les quêtes

Lorsque l’utilisateur demande la génération d’une quête ou une réflexion sur une quête, les informations suivantes peuvent être utilisées pour un traitement externe via Firebase Functions :

- Titre du journal
- Contenu du journal ou contenu de la réflexion
- Catégorie
- Niveau de difficulté
- Quête sélectionnée
- Informations de synthèse du profil de quête

Ces informations sont utilisées pour la génération et l’évaluation de quêtes via l’API OpenAI.

Important :

- Le contenu du journal concerné n’est utilisé pour un traitement externe que lorsque la fonctionnalité de quête est utilisée.
- Selon la configuration actuelle du projet, aucun code stockant des journaux de quêtes dans une collection distincte `questLogs` n’est utilisé.

## 5. Services tiers et traitement confié à des tiers

### 5-1. Google Firebase

Finalité :

- Authentification (Firebase Authentication)
- Stockage dans Firestore
- Exécution de Cloud Functions

Informations pouvant être traitées :

- UID, adresse e-mail et statut d’authentification
- Données de journal enregistrées manuellement par l’utilisateur
- Données de requête liées aux quêtes

### 5-2. OpenAI

Finalité :

- Génération de quêtes
- Réflexion sur les quêtes et évaluation de leur achèvement

Informations pouvant être traitées :

- Titre / contenu du journal
- Texte de la quête
- Niveau de difficulté et catégorie
- Contenu de réflexion saisi par l’utilisateur
- Informations de synthèse du profil de quête

### 5-3. Google AdMob / UMP

Finalité :

- Fourniture de publicités bannière, interstitielles et avec récompense
- Gestion du consentement publicitaire et des options de confidentialité

Informations pouvant être traitées :

- Identifiants publicitaires
- Informations sur l’appareil et le réseau
- Informations sur les interactions publicitaires
- Statut du consentement

## 6. Avis relatif aux transferts internationaux

L’application peut traiter des données à caractère personnel ou des informations connexes en dehors du pays de l’utilisateur dans les cas suivants :

| Élément | Détails |
|---|---|
| Destinataires | Google LLC, OpenAI et les opérateurs d’infrastructure associés |
| Pays de destination | États-Unis, etc. |
| Moment du transfert | Lors de la connexion, de la génération/réflexion sur les quêtes, des demandes publicitaires et du traitement du consentement |
| Méthode de transfert | Communication réseau chiffrée |
| Finalité du transfert | Authentification, stockage des données, traitement serverless, génération/évaluation de quêtes par IA et fourniture de publicités |

## 7. Durée de conservation et d’utilisation

L’application conserve les informations selon les critères suivants :

- Informations locales du journal / des paramètres : jusqu’à leur suppression par l’utilisateur ou la désinstallation de l’application
- Informations du compte Firebase : tant que l’utilisateur conserve son compte
- Données stockées dans Firestore : tant que l’utilisateur conserve les éléments enregistrés
- Données liées au traitement des requêtes de quête : dans la mesure nécessaire au traitement serverless
- Données liées à la publicité / au consentement : conformément à la politique de chaque prestataire externe

En outre, le projet actuel comprend la logique de nettoyage automatique suivante :

- Nettoyage, après une certaine période, des comptes d’utilisateurs anonymes ainsi que des données Firestore des sous-collections utilisateur
- Nettoyage des comptes d’utilisateurs réguliers inactifs pendant une longue période ainsi que des données Firestore des sous-collections utilisateur

Toutefois, leur application effective dans l’environnement de production peut varier selon l’état du déploiement et la configuration du serveur.

## 8. Avis sur le verrouillage de l’application et le chiffrement local

L’application propose une fonctionnalité distincte de `Diary App Lock`.

- La phrase secrète du verrouillage de l’application est distincte du mot de passe du compte.
- La phrase secrète du verrouillage de l’application est utilisée pour le chiffrement et le déchiffrement local du journal.
- Même si une phrase secrète incorrecte est saisie, l’application elle-même peut ne pas être entièrement bloquée ; à la place, certains contenus du journal peuvent rester illisibles.
- Certains journaux peuvent être chiffrés séparément selon la phrase secrète utilisée au moment de l’écriture ou du déverrouillage temporaire.

Les utilisateurs doivent conserver leur phrase secrète en lieu sûr. En cas de perte, la récupération de certaines données locales peut être difficile.

## 9. Avis sur les notifications de quête

Si l’utilisateur active les notifications de quête, des notifications locales peuvent être programmées pour chaque journal contenant une quête en cours.

- La programmation est principalement gérée par la planification interne de l’appareil.
- Selon la configuration actuelle du projet, aucune structure n’a été confirmée dans laquelle le texte source du journal serait transmis périodiquement à un serveur central uniquement à des fins de notification.

## 10. Avis sur l’utilisation des autorisations

L’application peut utiliser les autorisations suivantes afin de fournir ses fonctionnalités :

- `INTERNET` : communication avec Firebase, OpenAI et les SDK publicitaires
- `com.google.android.gms.permission.AD_ID` : utilisation des identifiants publicitaires
- `POST_NOTIFICATIONS` : affichage des notifications de quête
- `RECEIVE_BOOT_COMPLETED` : restauration des notifications programmées après redémarrage de l’appareil

Les autorisations sont utilisées uniquement dans la mesure nécessaire à l’exécution des fonctionnalités concernées.

## 11. Droits de la personne concernée et modalités d’exercice

Les utilisateurs peuvent exercer les droits suivants :

- Accéder aux données dans l’application, les modifier et les supprimer
- Supprimer ou écraser les données stockées dans le cloud
- Demander la déconnexion et la suppression du compte
- Modifier les options de confidentialité liées à la publicité
- Désactiver les autorisations de notification

Modalités d’exercice :

- Supprimer ou modifier directement les journaux dans l’application
- Supprimer l’application ou réinitialiser les données locales
- Se déconnecter du compte et demander séparément sa suppression
- Modifier les notifications, les identifiants publicitaires et les autorisations dans les paramètres de l’appareil
- E-mail de contact : [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

## 12. Mesures de sécurité

L’application applique ou peut appliquer les mesures de protection suivantes :

- Communication fondée sur HTTPS
- Verrouillage et chiffrement local de l’application de journal
- Stockage séparé des valeurs de vérification de la phrase secrète
- Utilisation de Firebase Authentication
- Demande d’autorisations minimales

Cependant, des risques peuvent survenir en fonction de l’état de sécurité de l’appareil de l’utilisateur, notamment en cas de root, jailbreak, malware ou utilisation d’un appareil partagé.

## 13. Données à caractère personnel des enfants

L’application n’est pas conçue comme un service principalement destiné aux enfants. Toutefois, des options liées à l’âge dans UMP peuvent être appliquées lors du traitement des publicités et du consentement.

## 14. Modifications de la présente politique

La présente Politique peut être révisée en raison de modifications de la législation, des services tiers ou des fonctionnalités de l’application.

- Dernière mise à jour pour la version actuelle : **2026-04-19**

## 15. Contact

- Développeur : frog-im
- E-mail : [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- Guide de suppression de compte : [Instructions de suppression](https://docs.google.com/forms/d/e/1FAIpQLSexIrSPRwSmVG5aU-Mp0wq0uRyXTh2Xh9Gag3Y4QBisWmFZWw/viewform?usp=dialog)

