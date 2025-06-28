# Backend – Application Mobile du Maintenancier

Ce dépôt contient le code source du **backend** de l'application mobile destinée aux maintenanciers. Il est développé avec **Node.js** et **Express.js** et assure la gestion de l’authentification, des dispositifs, des tâches, du profil utilisateur et des services de support.

## ⚙️ Fonctionnalités principales

- **Authentification**
  - Connexion via email et mot de passe
  - Création de compte avec vérification par code OTP
  - Gestion de session via JWT

- **Dashboard (Page d'accueil)**
  - Nombre total de dispositifs gérés par le maintenancier
  - Nombre de dispositifs connectés
  - Nombre de dispositifs déconnectés/en panne
  - Liste restreinte de dispositifs (nom, statut, adresse MAC)
  - Accès aux détails et à l’historique d’interventions

- **Liste des Tâches**
  - Affichage des tâches générées automatiquement en cas de panne
  - Prise en charge d’une tâche avec saisie de date d’intervention prévue
  - Marquage d’une tâche comme terminée avec description d’intervention

- **Gestion du Profil**
  - Visualisation et modification des informations personnelles
  - Changement du mot de passe
  - Suppression du compte

- **Assistance & Support**
  - Accès à une FAQ
  - Informations de contact pour le support


## 🧪 Lancer le serveur

```bash
# Installer les dépendances
npm install

# Créer un fichier .env avec le contenu suivant:
DATABASE_URL = "postgresql://read_write_only_user:npg_R2FsboC5DWIq@ep-white-tree-a2t10s0c.eu-central-1.aws.neon.tech/oramadb_prjt?sslmode=require" 
EMAIL_PASS = "wuba jczu ofsr zwyg"
EMAIL_USER = "li_louni@esi.dz"

# Démarrer le serveur avec cette commande:
npm run dev 0.0.0.0:3003
