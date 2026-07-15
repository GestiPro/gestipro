# GestiPro

> **La gestion simple et efficace pour les professionnels**

GestiPro est une solution SaaS française destinée aux artisans, indépendants et petites entreprises afin de simplifier leur gestion administrative quotidienne.

L'objectif est de proposer un outil moderne permettant de gérer facilement les devis, factures, clients, paiements et collaborations, tout en restant simple à utiliser.

---

# 🎯 Objectifs du projet

GestiPro vise à :

* Réduire le temps passé sur les tâches administratives.
* Centraliser les documents importants.
* Faciliter les échanges entre professionnels, clients et comptables.
* Proposer une solution adaptée aux besoins des petites structures.
* Respecter les normes françaises de facturation.

---

# 👥 Types d'utilisateurs

## 👑 Administrateur plateforme

Gestionnaire de GestiPro.

Permissions :

* Gestion des entreprises clientes.
* Gestion des abonnements.
* Gestion du support.
* Suivi des statistiques globales.
* Maintenance de la plateforme.

---

## 🏢 Propriétaire d'entreprise

Responsable du compte professionnel.

Permissions :

* Gestion de l'entreprise.
* Gestion des utilisateurs.
* Création des devis.
* Création des factures.
* Gestion des clients.
* Gestion des paiements.
* Accès aux statistiques.
* Invitation d'un comptable.

---

## 👷 Collaborateur

Membre de l'entreprise.

Permissions configurables :

* Création de devis.
* Gestion des clients.
* Création de factures.
* Consultation des documents.
* Accès limité aux informations financières.

---

## 📊 Comptable

Utilisateur externe ayant accès aux données comptables.

Permissions :

* Consultation des factures.
* Export comptable.
* Consultation des paiements.
* Téléchargement des documents.
* Suivi de la TVA.

Restrictions :

* Pas de suppression de documents.
* Pas d'accès aux paramètres de l'entreprise.
* Pas de gestion des utilisateurs.

---

## 👤 Client

Client final de l'entreprise.

Permissions :

* Consultation des devis.
* Acceptation ou refus des devis.
* Téléchargement des factures.
* Consultation de l'historique.
* Paiement en ligne (future fonctionnalité).

---

# 🧩 Fonctionnalités principales

## Gestion des entreprises

* Création d'une entreprise.
* Informations légales.
* Coordonnées.
* Paramètres de facturation.
* Logo et personnalisation des documents.

---

## Gestion des utilisateurs

* Invitation d'utilisateurs.
* Gestion des rôles.
* Gestion des permissions.
* Historique des actions.

---

## Gestion des clients

* Création de fiches clients.
* Historique des échanges.
* Historique des devis.
* Historique des factures.

---

## Gestion des prestations

Catalogue permettant de créer :

* Produits.
* Services.
* Tarifs.
* TVA associée.

---

# 📄 Devis

Fonctionnalités :

* Création rapide.
* Ajout de prestations.
* Calcul automatique.
* Gestion de la TVA.
* Génération PDF.
* Envoi par e-mail.
* Acceptation par le client.

Statuts :

```
BROUILLON
ENVOYE
ACCEPTE
REFUSE
EXPIRE
```

---

# 🧾 Factures

Fonctionnalités :

* Création depuis un devis.
* Numérotation automatique.
* Génération PDF.
* Suivi des paiements.
* Gestion des échéances.
* Gestion des avoirs.

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

# 💶 Paiements

Gestion :

* Paiement reçu.
* Date de paiement.
* Moyen de paiement.
* Montant.
* Historique.

---

# 📊 Tableau de bord

Informations principales :

* Chiffre d'affaires.
* Factures en attente.
* Paiements reçus.
* Devis en attente.
* Évolution mensuelle.
* Clients principaux.

---

# 🔐 Sécurité

Le projet devra intégrer :

* Authentification sécurisée.
* Hashage des mots de passe.
* Gestion des permissions.
* Protection CSRF.
* Journalisation des actions.
* Isolation des données entre entreprises.

---

# 🇫🇷 Conformité française

Prévoir :

* Mentions obligatoires sur les factures.
* Numérotation conforme.
* Gestion TVA.
* Gestion des avoirs.
* Conservation des documents.
* Préparation à la facturation électronique.

---

# 🏗️ Architecture technique envisagée

## Backend

* Symfony 7
* Doctrine ORM
* PostgreSQL / MySQL
* Symfony Security
* Symfony Mailer
* Symfony Messenger

## Frontend

* Twig
* Bootstrap ou Tailwind CSS
* JavaScript

## Génération documentaire

* Génération PDF des devis et factures.
* Modèles personnalisables.

---

# 🗃️ Entités principales

```
User
 |
 |--- Role
 |
Company
 |
 |--- Customer
 |
 |--- Quote
 |
 |--- Invoice
 |
 |--- Payment
 |
 |--- Product
 |
 |--- Document
 |
 |--- ActivityLog
```

---

# 🚀 Roadmap

## Version 1 - MVP

* Authentification.
* Création entreprise.
* Gestion clients.
* Création devis.
* Génération PDF.
* Création factures.
* Suivi des paiements.

## Version 2

* Espace client.
* Espace comptable.
* Invitations utilisateurs.
* Permissions avancées.
* Historique des actions.

## Version 3

* Facturation électronique.
* Signature électronique.
* Paiement en ligne.
* API.
* Application mobile.

---

# 💡 Vision

GestiPro n'est pas seulement un outil de facturation.

C'est un assistant de gestion permettant aux professionnels de piloter leur activité simplement, avec tous leurs documents et collaborateurs réunis au même endroit.

---

**GestiPro — Votre activité, simplement maîtrisée.**
