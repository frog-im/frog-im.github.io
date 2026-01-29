---
title: Politique de confidentialité | Power lucky lotto
description: Politique de confidentialité de Power lucky lotto (Français)
lang: fr
last_updated: 2026-01-29
---

# Politique de confidentialité (Power lucky lotto)

- **Nom de l’application :** Power lucky lotto  
- **Développeur :** frog-im  
- **Contact :** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)  
- **Date d’entrée en vigueur :** 2026-01-29  

> Cette politique est rédigée en tenant compte des lois applicables (PIPA coréenne, RGPD/UK GDPR, FADP suisse, lois étatiques américaines, etc.).  
> Si votre région impose des exigences spécifiques, elles prévalent.

---

## 1. Objet et champ d’application

Power lucky lotto est une application de gestion de jeux de loterie et de consultation d’historique. Principales fonctionnalités :

- Sélection/configuration du pays et du jeu (ex. KR 6/45, US Powerball)  
- Génération/enregistrement de numéros et consultation des journaux (logs)  
- Consultation et suppression de tables de logs (liste/détail)  
- Édition/gestion de données de résultats via JSON (statistiques/visualisation)  
- Publicités (dont publicités récompensées) et gestion du consentement (si requis)

L’application **ne nécessite pas de compte** et, par défaut, **n’envoie pas vos données aux serveurs du développeur**.  
La plupart des traitements ont lieu **sur l’appareil**.

Cependant, pour la **publicité**, la **gestion du consentement** et la **conformité**, des SDK tiers tels que  
**Google Mobile Ads SDK (AdMob)** et **Google UMP** peuvent collecter et traiter certaines données (p. ex. identifiants publicitaires).

---

## 2. Types de données traitées

### 2-1) Données stockées localement sur l’appareil

#### (1) Paramètres (SharedPreferences)

| Catégorie | Clé (exemple) | Finalité | Stockage | Suppression |
|---|---|---|---|---|
| Configuration terminée | `setup_done` | État de configuration initiale | SharedPreferences | Suppression des données/désinstallation |
| Historique des pays | `selected_countries` | Pays récemment sélectionnés | Idem | Idem |
| Pays actif | `active_country` | Pays actuellement sélectionné | Idem | Idem |
| Jeux sélectionnés | `selected_lotto_ids` | IDs des jeux cochés | Idem | Idem |
| Jeu actif | `active_lotto_id` | ID du jeu actif | Idem | Idem |
| **Sélection de l’heure seed (facultatif)** | `birth_datetime_iso` | Heure de référence seed choisie par l’utilisateur (peut servir de seed/personalisation) | Idem | Idem |

#### (2) Journaux (SQLite)

- Tables typiques : `log_...`  
- Champs possibles : `id`, `date_id` ou `date_text`, `choice1..choiceN`, `isFinger`

L’utilisateur peut consulter et supprimer ces données dans l’application.

#### (3) Fichiers JSON (par jeu)

- Exemple : `game_json/<gameId>.json`  
- Utilité : gestion/édition par l’utilisateur de données de tirages/résultats (statistiques/visualisation)

---

### 2-2) Publicité, consentement et données associées (SDK tiers)

AdMob et Google UMP peuvent traiter :

- Identifiant publicitaire (AAID/IDFA)  
- Informations basées sur IP, localisation approximative, réseau  
- Informations appareil/app (versions, langue, diagnostics)  
- Interactions publicitaires (impressions, clics, récompense)  
- Choix/état de consentement (UMP)

---

## 3. Durée de conservation

- Paramètres locaux : jusqu’à suppression des données ou désinstallation  
- Logs SQLite : jusqu’à suppression par l’utilisateur ou désinstallation/suppression des données  
- Fichiers JSON : stockés dans le répertoire documents de l’app; exports/sauvegardes relèvent de l’utilisateur  
- Données publicitaires/consentement : selon politiques Google et lois applicables

---

## 4. Tiers et transferts internationaux

| Élément | Détails |
|---|---|
| Destinataires | Google LLC, affiliés et sous-traitants |
| Destinations | États-Unis et autres régions d’infrastructure Google |
| Finalité | Diffusion/mesure pub, anti-fraude, consentement, conformité |
| Données | ID pub, infos IP, infos appareil/app, interactions, consentement |
| Conservation | Selon politiques Google et lois |
| Impact si refus | Publicités personnalisées limitées, pub non personnalisée ou moins de pub |

---

## 5. Vos droits

Selon la loi, vous pouvez disposer de droits (accès, rectification, suppression, limitation, opposition, portabilité, retrait du consentement).

- Ajuster pubs/consentement : via “Privacy Options” dans l’app (si disponible) ou paramètres du système (réinitialiser l’ID publicitaire, limiter la personnalisation).  
- Réinitialiser données locales : suppression des données de l’app ou désinstallation.

---

## 6. Données des enfants

L’application **n’est pas conçue pour les enfants**. L’usage de contrôles parentaux et de limites publicitaires au niveau du système est recommandé si nécessaire.

---

## 7. Sécurité

- Minimisation des données stockées localement  
- Traitements sur l’appareil lorsque possible  
- Transport sécurisé (TLS) pour les communications des SDK (selon leurs capacités)

---

## 8. Data safety (Google Play)

Le développeur s’efforce de maintenir les déclarations “Data safety” exactes et à jour lorsque les pratiques/SDK changent.

---

## 9. Open source

L’application peut utiliser des bibliothèques open source (icônes de pays, stockage, pub/consentement, UI).  
Les licences sont disponibles dans l’écran “Licences open source” (ou équivalent) de l’application.

---

## 10. Contact

- Email : [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)  
Merci d’indiquer “Power lucky lotto” dans votre message.

---

## 11. Modifications

Cette politique peut évoluer (lois, fonctionnalités, SDK, politique interne).  
Les changements mineurs seront publiés dans l’app ou sur cette page; les changements importants seront annoncés à l’avance si requis.
