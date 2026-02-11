# 🚀 Portfolio Moderne — React + Vite + TypeScript

> **En construction** — Refactorisation du portfolio de Jekyll vers une application React moderne.

Un portfolio professionnel moderne, interactif et performant. Construit avec React, Vite, TypeScript et Tailwind CSS. Déployé sur GitHub Pages.

## 📋 À propos du projet

Ce projet est à la fois un **portfolio personnel** ET une **vitrine de compétences techniques**. L'objectif est d'apprendre en faisant, en construisant une application web moderne qui démontre:

- ✅ Maîtrise de **React** (hooks, state, routing)
- ✅ **TypeScript** et types stricts
- ✅ **Tailwind CSS** et responsive design
- ✅ **Animations fluides** avec Framer Motion
- ✅ **Architecture propre** et maintenable
- ✅ **CI/CD** avec GitHub Actions
- ✅ **SEO et accessibilité** web

## 🛠️ Stack technologique

```
Frontend:
  - React 18+ avec TypeScript
  - Vite (bundler ultra-rapide)
  - Tailwind CSS (utility-first)
  - Framer Motion (animations)
  - React Router (SPA routing)

Backend/Services:
  - EmailJS ou Formspree (formulaires sans serveur)

Deployment:
  - GitHub Pages (statique)
  - GitHub Actions (CI/CD)
```

## 📁 Structure du projet (future)

```
portfolio-react/
├── src/
│   ├── components/        # Composants réutilisables
│   │   ├── Layout.tsx
│   │   ├── Navbar.tsx
│   │   ├── Footer.tsx
│   │   └── ui/           # Button, Card, Badge, etc.
│   ├── pages/            # Pages (routed)
│   │   ├── Home.tsx
│   │   ├── About.tsx
│   │   ├── Projects.tsx
│   │   ├── ProjectDetail.tsx
│   │   └── Contact.tsx
│   ├── hooks/            # Custom hooks
│   ├── context/          # Context API (dark mode, etc.)
│   ├── data/             # Données statiques (projets, skills)
│   ├── App.tsx           # Routing
│   └── main.tsx          # Entry point
├── public/               # Assets statiques
├── tailwind.config.ts    # Config Tailwind
├── vite.config.ts        # Config Vite
├── tsconfig.json         # Config TypeScript
├── package.json          # Dépendances
└── .github/
    └── workflows/
        └── deploy.yml    # GitHub Actions
```

## 🚀 Démarrage rapide

```bash
# Cloner le repo
git clone https://github.com/[TON_USERNAME]/portfolio-react.git
cd portfolio-react

# Installer les dépendances
npm install

# Démarrer le serveur de dev
npm run dev

# Build pour production
npm run build

# Preview production
npm run preview
```

## 📖 Plan de développement

Voir [REFACTOR_PLAN.md](REFACTOR_PLAN.md) pour le plan détaillé en ~22 étapes.

**Phases:**

1. **Phase 0** — Setup (Vite, React, TypeScript, GitHub Actions)
2. **Phase 1** — Structure de base (Layout, Navbar, Footer, Routing)
3. **Phase 2** — Design System (Colors, Components, Dark mode)
4. **Phase 3** — Pages (Accueil, À propos, Projets, Détails, Contact)
5. **Phase 4** — Polish (Animations, Scroll effects, Easter eggs)
6. **Phase 5** — Production (SEO, Performance, A11y, Deploy)

## 🎯 Prochaines étapes

- [ ] **Phase 0.1** — Initialiser Vite + React + TypeScript
- [ ] **Phase 0.2** — Configurer Tailwind CSS
- [ ] **Phase 0.3** — Nettoyer le boilerplate
- [ ] **Phase 0.4** — Setup GitHub Actions

## 📝 Notes

- Ce projet est une **expérience d'apprentissage**. Le code sera progressivement amélioré et optimisé.
- Chaque étape inclut des concepts à apprendre et des défis à relever.
- Les contributions sont bienvenues ! 🎉

## 📧 Contact

Pour toute question sur ce projet ou mon parcours, consultez la page Contact du portfolio.

---

**Status**: 🔧 En cours de refactorisation  
**Last updated**: Février 2026
