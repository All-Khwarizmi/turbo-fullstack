# Turbo Full Stack Starter

Un starter kit moderne pour applications full stack, utilisant une architecture monorepo avec TurboRepo.

## 🏗️ Architecture

```bash
.
├── apps/
│   ├── api/           # Backend NestJS
│   └── web/          # Frontend React + Vite (à venir)
├── packages/
│   ├── ui/           # Composants UI partagés
│   ├── types/        # Types/interfaces partagés
│   └── config/       # Configurations partagées
└── README.md         # Ce fichier
```

## 🚀 Quick Start

```bash
# Installation des dépendances
pnpm install

# Démarrer la base de données
docker-compose up -d

# Setup de la base de données
cd apps/api && pnpm run db:setup

# Démarrer le développement
pnpm dev
```

## 📚 Stack Technique

### Backend (NestJS)
- NestJS pour l'API REST
- PostgreSQL avec requêtes SQL natives (pas d'ORM)
- Docker pour la conteneurisation
- Swagger pour la documentation API

### Frontend (à venir)
- React + Vite
- Redux Toolkit
- shadcn/ui
- React Router

### Outils & Qualité
- TypeScript
- ESLint & Prettier
- Tests avec Vitest
- Docker & Docker Compose
- CI/CD avec GitHub Actions

## 📖 Documentation Détaillée
- [Documentation API](./apps/api/README.md)
- [Documentation Frontend](./apps/web/README.md)
- [Guide Base de Données](./apps/api/db/README.md)
- [Guide Docker](./docs/docker.md)