# GestiPro

> **La plateforme open-source de gestion pour les professionnels**

![GestiPro Logo](docs/assets/logo.png)

GestiPro est une solution open-source de gestion d'entreprise conçue pour les artisans, indépendants et petites structures.

Contrairement aux solutions SaaS classiques, GestiPro est pensé pour être **installé, personnalisé et intégré directement à l'écosystème numérique de chaque entreprise**.

Chaque entreprise dispose de son propre espace professionnel accessible depuis son domaine ou sous-domaine.

Exemple :

```
https://gestipro.stephaneauve.fr
```

L'entreprise conserve ainsi son identité, ses données et son environnement de travail.

---

# 🎯 Vision du projet

L'objectif de GestiPro est de proposer une alternative simple, moderne et transparente aux logiciels de gestion propriétaires.

GestiPro permet aux professionnels de :

* gérer leur activité ;
* suivre leurs clients ;
* créer leurs devis et factures ;
* collaborer avec leurs équipes ;
* donner un accès sécurisé à leurs clients et comptables ;
* conserver la maîtrise de leurs données.

---

# ✨ Fonctionnalités principales

## 📄 Gestion commerciale

### Devis

* Création de devis professionnels.
* Calcul automatique des montants.
* Gestion de la TVA.
* Génération PDF.
* Envoi au client.
* Acceptation ou refus en ligne.
* Historique des modifications.

Statuts :

```
BROUILLON
ENVOYE
ACCEPTE
REFUSE
EXPIRE
```

---

### Factures

* Création depuis un devis.
* Numérotation automatique.
* Génération PDF.
* Suivi des règlements.
* Gestion des échéances.
* Gestion des avoirs.
* Historique complet.

Statuts :

```
BROUILLON
EMISE
ENVOYEE
PAYEE
PARTIELLEMENT_PAYEE
EN_RETARD
ANNULEE
```

---

# 👥 Gestion des utilisateurs

GestiPro possède un système complet de rôles et permissions.

## 👑 Administrateur système

Administrateur de l'installation GestiPro.

Permissions :

* Configuration globale.
* Gestion des modules.
* Gestion des mises à jour.
* Gestion technique.
* Surveillance système.

---

## 🏢 Administrateur entreprise

Responsable de l'entreprise.

Permissions :

* Gestion de l'entreprise.
* Gestion des utilisateurs.
* Gestion des clients.
* Gestion des documents.
* Paramétrage de la facturation.

---

## 👷 Collaborateur

Membre de l'entreprise.

Permissions personnalisables :

* Création de devis.
* Gestion des clients.
* Création de factures.
* Consultation des documents.

---

## 📊 Comptable

Accès dédié aux professionnels de la comptabilité.

Permissions :

* Consultation des factures.
* Export comptable.
* Consultation des paiements.
* Accès aux documents nécessaires.

Restrictions :

* Pas de suppression.
* Pas de modification des paramètres entreprise.

---

## 👤 Client

Espace client sécurisé.

Fonctionnalités :

* Consultation des devis.
* Acceptation électronique.
* Téléchargement des factures.
* Consultation des documents.
* Suivi des paiements.

---

# 🌐 Intégration aux sites internet

GestiPro est conçu pour fonctionner avec les sites professionnels existants.

Exemple :

Site public :

```
https://www.exemple.fr
```

Espace gestion :

```
https://gestipro.exemple.fr
```

Les clients peuvent :

* demander un devis ;
* suivre leur dossier ;
* récupérer leurs documents ;
* communiquer avec l'entreprise.

---

# 🎨 Personnalisation

Chaque installation peut être adaptée à l'entreprise.

Personnalisation :

* Logo.
* Couleurs.
* Nom de l'entreprise.
* Modèles de documents.
* Mentions légales.
* Domaine personnalisé.

Exemple :

```
GestiPro

SARL Stéphane Auvé BTP
```

---

# 🔐 Sécurité

GestiPro intègre :

* Authentification sécurisée.
* Gestion fine des permissions.
* Protection CSRF.
* Hashage des mots de passe.
* Journalisation des actions.
* Isolation des données.
* Sauvegardes.

Chaque entreprise possède un environnement indépendant.

---

# 🇫🇷 Conformité française

GestiPro est conçu pour respecter les besoins des entreprises françaises :

* Mentions obligatoires des documents.
* Numérotation des factures.
* Gestion TVA.
* Gestion des avoirs.
* Conservation des documents.
* Préparation à la facturation électronique.

---

# 🏗️ Architecture technique

## Backend

* Symfony 7
* PHP 8.3+
* Doctrine ORM
* PostgreSQL / MySQL
* Symfony Security
* Symfony Messenger

## Frontend

* Twig
* JavaScript
* Bootstrap / Tailwind CSS

## Documents

* Génération PDF.
* Modèles personnalisables.
* Archivage documentaire.

---

# 🧩 Architecture modulaire

GestiPro est conçu avec une approche par modules.

```
GestiPro

├── Core
│   ├── Utilisateurs
│   ├── Permissions
│   └── Configuration
│
├── CRM
│   ├── Clients
│   └── Contacts
│
├── Commercial
│   ├── Devis
│   └── Factures
│
├── Paiements
│
├── Documents
│
├── Comptabilité
│
├── Portail Client
│
└── API
```

---

# 🗃️ Principales entités

```
User

Company

Role

Permission

Customer

Contact

Product

Quote

Invoice

Payment

Document

ActivityLog

Configuration
```

---

# 🚀 Installation

Exemple :

```bash
git clone https://github.com/gestipro/gestipro.git

composer install

php bin/console doctrine:migrations:migrate

symfony server:start
```

---

# 🔄 Système de mises à jour

Chaque installation peut recevoir :

* mises à jour du cœur ;
* nouveaux modules ;
* correctifs de sécurité ;
* évolutions réglementaires.

---

# 🛣️ Roadmap

## Version 1.0

* Authentification.
* Gestion entreprise.
* Gestion utilisateurs.
* Clients.
* Devis.
* Factures.
* PDF.
* Permissions.

## Version 1.5

* Portail client.
* Espace comptable.
* Journal d'activité.
* Personnalisation avancée.

## Version 2.0

* Facturation électronique.
* Signature électronique.
* API publique.
* Marketplace de modules.
* Applications mobiles.

---

# 🤝 Philosophie Open Source

GestiPro est construit autour de principes simples :

* Les données appartiennent aux entreprises.
* Le logiciel doit rester transparent.
* Les professionnels doivent pouvoir choisir leur hébergement.
* La simplicité doit primer sur la complexité.

---

# 📜 Licence

À définir.

---

# 📬 Contribution

Les contributions sont les bienvenues :

* Développement.
* Documentation.
* Traductions.
* Suggestions.
* Tests.

---

# GestiPro

**Votre entreprise. Vos données. Votre outil.**
