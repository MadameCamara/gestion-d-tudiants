# 🎓 Gestion des Inscriptions des Étudiants

Ce projet est une application web full stack permettant la gestion des inscriptions d'étudiants. Il est construit avec **Laravel** pour le backend (API RESTful) et **Angular** pour le frontend (interface utilisateur).

---

## 📁 Structure du projet

```
gestion-inscriptions/
├── backend-laravel/      # Backend Laravel (API)
└── frontend-angular/     # Frontend Angular (UI)
```

---

## 🔧 Prérequis

- PHP >= 8.1
- Composer
- Node.js & npm
- Angular CLI (`npm install -g @angular/cli`)
- MySQL ou MariaDB
- (optionnel) Laragon ou XAMPP pour environnement local

---

## 🚀 Installation du backend Laravel

```bash
cd backend-laravel
composer install
cp .env.example .env
php artisan key:generate
```

### 🔧 Configuration de la base de données

Dans `.env`, configure :

```env
DB_DATABASE=inscription
DB_USERNAME=root
DB_PASSWORD=
```

Puis exécute :

```bash
php artisan migrate
php artisan serve
```

➡️ L'API sera accessible sur : `http://localhost:8000/api/students`

---

## 🚀 Installation du frontend Angular

```bash
cd frontend-angular
npm install
ng serve
```

➡️ L’interface Angular sera accessible sur : `http://localhost:4200`

---

## 📡 Fonctionnalités

- Création d’étudiant
- Affichage de la liste des étudiants
- Modification des données
- Suppression d’un étudiant

---

## 🔗 Routes API Laravel

| Méthode | Endpoint              | Action                |
|---------|------------------------|------------------------|
| GET     | `/api/students`        | Lister tous les étudiants |
| POST    | `/api/students`        | Ajouter un étudiant       |
| GET     | `/api/students/{id}`   | Voir un étudiant          |
| PUT     | `/api/students/{id}`   | Modifier un étudiant      |
| DELETE  | `/api/students/{id}`   | Supprimer un étudiant     |

---

## 🤝 Auteurs & contribution

Projet réalisé dans le cadre de la formation Full Stack Developer - Talent4Startups 2025.

---

## 🛠️ À venir (suggestions)

- Authentification JWT
- Recherche et tri d’étudiants
- Pagination