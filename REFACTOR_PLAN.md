# 📋 Plan de Refactor — Portfolio Jekyll → React + Vite

## 🎯 Objectif

Transformer le portfolio Jekyll statique en une **application React moderne** (Vite + React + TypeScript)
deployée sur GitHub Pages. Le portfolio lui-même devient une **vitrine de compétences**.

## 💡 Stack technologique choisi

| Technologie                   | Raison                                                            |
| ----------------------------- | ----------------------------------------------------------------- |
| **Vite + React + TypeScript** | Moderne, performant, apprendre React + TS (compétences clés 2026) |
| **Tailwind CSS**              | Utility-first, productif, responsive facile, standard industrie   |
| **Framer Motion**             | Animations fluides pour un portfolio vivant                       |
| **React Router**              | Navigation SPA multi-pages                                        |
| **EmailJS ou Formspree**      | Formulaire contact sans backend (GitHub Pages compatible)         |
| **GitHub Actions**            | CI/CD automatique, déploiement sur GitHub Pages                   |

> **Pourquoi pas Next.js ?** Next est excellent, mais pour un site 100% statique sur GitHub Pages, Vite + React est plus léger, tu apprends les fondamentaux sans "magie", et c'est trivial à déployer.

---

## 🗓️ Plan de travail en phases

### 🔧 Phase 0 — Setup (Fondations)

Initialiser le projet avec tous les outils nécessaires.

| Étape   | Titre                     | Description                                              | Tu apprends                                 |
| ------- | ------------------------- | -------------------------------------------------------- | ------------------------------------------- |
| **0.1** | Init Vite + React + TS    | `npm create vite@latest` avec template React + TS        | Scaffolding moderne, structure projet React |
| **0.2** | Installation Tailwind CSS | Config Tailwind, @layer directives, JIT mode             | Utility-first CSS, theming, config          |
| **0.3** | Nettoyage du boilerplate  | Supprimer App.css, Counter.tsx, etc. Garder la structure | Comprendre ce que génère Vite               |
| **0.4** | Setup GitHub Actions      | Créer workflow YAML pour déploiement automatique         | CI/CD, YAML, GitHub Pages statique          |

---

### 🧱 Phase 1 — Structure de base (Squelette)

Mettre en place la navigation et le layout principal.

| Étape   | Titre                | Description                                                   | Tu apprends                              |
| ------- | -------------------- | ------------------------------------------------------------- | ---------------------------------------- |
| **1.1** | Install React Router | `npm install react-router-dom` et setup routes basiques       | Routing SPA, navigation client-side      |
| **1.2** | Composant `Layout`   | Créer composant Layout avec `<Outlet />` pour Header + Footer | Composants réutilisables, outlet pattern |
| **1.3** | Navbar responsive    | Navbar avec hamburger menu (mobile), menu desktop             | State React, responsive design Tailwind  |
| **1.4** | Footer               | Footer avec liens sociaux, copyright, liens rapides           | Composants statiques, listes             |

---

### 🎨 Phase 2 — Design System (Identité visuelle)

Définir l'identité visuelle et les composants réutilisables.

| Étape   | Titre                    | Description                                                           | Tu apprends                             |
| ------- | ------------------------ | --------------------------------------------------------------------- | --------------------------------------- |
| **2.1** | Palette couleurs + typo  | Définir couleurs primaire/secondaire/accent dans `tailwind.config.ts` | Design tokens, theming Tailwind         |
| **2.2** | Dark/Light mode toggle   | Context API + localStorage pour persistance                           | Context API, localStorage, state global |
| **2.3** | Composants réutilisables | Créer Button, Card, Badge, Section avec TypeScript props              | Props TypeScript, composition, DRY      |

---

### 📄 Phase 3 — Pages (Contenu)

Construire les pages principales du portfolio.

| Étape   | Titre                     | Description                                                   | Tu apprends                                    |
| ------- | ------------------------- | ------------------------------------------------------------- | ---------------------------------------------- |
| **3.1** | Page Accueil - Hero       | Hero section avec titre, sous-titre, CTA. Animation au scroll | Framer Motion basics, first impression         |
| **3.2** | Page Accueil - Skills     | Section compétences avec liste des technologies               | Array.map(), composants dynamiques             |
| **3.3** | Page À propos             | Bio + timeline du parcours (formation, expériences)           | Composants chronologiques, données structurées |
| **3.4** | Page Projets - Liste      | Grid de cards pour tous les projets                           | Array.map(), Card component, props             |
| **3.5** | Page Projets - Filtrage   | Boutons pour filtrer par technologie/catégorie                | useState, filtering logic, UX interactive      |
| **3.6** | Page Projet détaillé      | Route dynamique `/projects/:id` avec détails complets         | useParams(), route params, lazy loading        |
| **3.7** | Page Contact - Formulaire | Formulaire avec validation et intégration EmailJS/Formspree   | Forms React, validation, API calls             |

---

### ✨ Phase 4 — Polish & Interactivité (Wow effect)

Ajouter les touches finales et interactions engageantes.

| Étape   | Titre                           | Description                                            | Tu apprends                                   |
| ------- | ------------------------------- | ------------------------------------------------------ | --------------------------------------------- |
| **4.1** | Animations transitions          | Transitions fluides entre les pages avec Framer Motion | AnimatePresence, page transitions             |
| **4.2** | Scroll animations               | Les éléments apparaissent/bougent au scroll            | Intersection Observer ou Framer Motion scroll |
| **4.3** | Effet typing                    | Texte qui s'écrit progressivement sur la hero          | Custom hooks, useEffect, setInterval          |
| **4.4** | Easter egg ou feature originale | Feature surprise ou fun (à définir ensemble)           | Créativité + technique combinée               |

---

### 🚀 Phase 5 — Production (Ship it!)

Optimiser pour production et déployer.

| Étape   | Titre                  | Description                                               | Tu apprends                             |
| ------- | ---------------------- | --------------------------------------------------------- | --------------------------------------- |
| **5.1** | SEO & Meta tags        | React Helmet, Open Graph, sitemap.xml                     | React Helmet, SEO for SPA, Open Graph   |
| **5.2** | Performance            | Lazy loading composants, optimisation images (WebP)       | React.lazy(), Suspense, images modernes |
---

## 📊 Résumé

- **Total étapes**: ~30 étapes granulaires
- **Phases**: 5 phases (Setup, Routing, Design, Pages, Animations, Production)
- **Durée estimée**: 20-30h de travail (45min-1h par étape)
- **Rythme suggéré**: 3-5 étapes par session de travail

---

## 🤝 Méthodologie de travail ensemble

À **chaque étape**, on suit ce processus:

1. **Explication courte** — Pourquoi on fait ça, ce qu'on va tester
2. **Développement** — Toi tu codes, je guide si nécessaire
3. **Test dans le navigateur** — On vérify ensemble que ça marche
4. **Commit** — On sauvegarde ce checkpoint
5. **Prochaine étape** — On move une fois que c'est solidifié

**Ton rôle**: Écrire le code, tester, poser des questions
**Mon rôle**: Guider, expliquer, aider au débogage, pas faire à ta place

**Important**: On ne passe à l'étape suivante que si tu vois le résultat fonctionner dans le navigateur.

---

## 🎓 Compétences que tu vas acquérir

À la fin de ce projet:

- ✅ **React** fondamentals (components, hooks, state, props)
- ✅ **TypeScript** (types, interfaces, strict mode)
- ✅ **Routing SPA** avec React Router
- ✅ **Tailwind CSS** (utility-first, responsive design)
- ✅ **Framer Motion** (animations, transitions)
- ✅ **GitHub Actions** et CI/CD
- ✅ **SEO et accessibility** web
- ✅ Un **portfolio impressionnant** 🚀

---

## 🚀 On démarre ?

**Phase 0.1 : Initialisation Vite + React + TypeScript**

Prêt ? 🎯

---

## 🤝 Philosophie de développement

**On code organique, pas en cascade.**

Chaque étape doit:
- ✅ Être **vraiment atomique** (une seule chose)
- ✅ Être **testable immédiatement** (tu vois le résultat dans le navigateur)
- ✅ Ne pas préparer d'infrastructure invisible
- ✅ S'avancer que quand c'est **fonctionnel et vérifiable**

**Pas de préparation invisible** comme:
- ❌ Installer des dépendances qui ne seront pas utilisées tout de suite
- ❌ Créer une structure de dossiers complète d'avance
- ❌ Écrire du code qu'on ne peut pas tester
- ❌ Commencer du styling avant que l'élément existe

**Le rythme:**
1. Créer quelque chose de petit
2. Vérifier que ça marche (voir dans le navigateur)
3. Commit
4. Passer au suivant

---

## 🗓️ Plan de travail — Étapes testables

### 🔧 Phase 0 — Setup (Fondations)

Les toutes premières briques du projet.

| Étape   | Titre                              | Description                                                    | Résultat visible                        |
| ------- | ---------------------------------- | -------------------------------------------------------------- | --------------------------------------- |
| **0.1** | Init Vite + React + TS             | `npm create vite@latest` → React template                      | Page par défaut Vite dans le navigateur |
| **0.2** | Vérifier que ça tourne             | `npm install` et `npm run dev` → tu vois la page               | ✅ App tourne sur localhost:5173        |
| **0.3** | Premier commit                     | `git add .` et `git commit`                                    | 📦 Checkpoint sauvegardé                |

---

### 🧱 Phase 1 — Premiers composants et routing

Construire le squelette avec routing et un premier layout.

| Étape   | Titre                       | Description                                                              | Résultat visible                                     |
| ------- | --------------------------- | ------------------------------------------------------------------------ | ---------------------------------------------------- |
| **1.1** | Installer React Router      | `npm install react-router-dom`                                           | Rien de visible encore (setup)                      |
| **1.2** | Créer 3 pages vides         | Home.tsx, About.tsx, Projects.tsx (juste du texte "Page X")              | Tu vois "Page Home" quand tu cliques sur les routes |
| **1.3** | Routing basique             | Créer App.tsx avec routes qui fonctionnent                               | Navigation entre pages (URLs changent)              |
| **1.4** | Composant Layout + Navbar   | Navbar en haut (avec liens), Outlet au milieu                            | Navbar visible sur toutes les pages                 |
| **1.5** | Footer simple               | Footer en bas de la page                                                 | Footer visible en bas                               |
| **1.6** | Commit checkpoint           | `git add .` et `git commit`                                              | 📦 SPA de base fonctionnelle                        |

---

### 🎨 Phase 2 — Design System minimal

Ajouter du style progressivement, seulement quand on l'utilise.

| Étape   | Titre                      | Description                                                           | Résultat visible                        |
| ------- | -------------------------- | --------------------------------------------------------------------- | --------------------------------------- |
| **2.1** | Installer Tailwind CSS     | `npm install -D tailwindcss postcss autoprefixer`                    | Rien encore (setup)                     |
| **2.2** | Configurer Tailwind        | `tailwind.config.ts`, `postcss.config.js`, importer dans main.css    | Rien encore (setup)                     |
| **2.3** | Styler la Navbar           | Ajouter des classes Tailwind à la Navbar (flex, bg, padding, etc.)   | Navbar styled et agréable               |
| **2.4** | Styler le Footer           | Ajouter des classes Tailwind au Footer                                | Footer styled                           |
| **2.5** | Layout global + spacing    | Conteneurs, padding, font de base pour tout le site                   | Site cohérent et aéré                   |
| **2.6** | Couleurs custom Tailwind    | Définir palette primaire/secondaire/accent dans config                | Application des couleurs au site        |
| **2.7** | Commit checkpoint          | `git add .` et `git commit`                                            | 📦 Design basique en place              |

---

### 📄 Phase 3 — Pages principales (contenu)

Construire chaque page au fur et à mesure, une par une.

| Étape   | Titre                           | Description                                                          | Résultat visible                      |
| ------- | ------------------------------- | -------------------------------------------------------------------- | ------------------------------------- |
| **3.1** | Hero section (Accueil)          | Titre, sous-titre, boutons CTA. Du texte et boutons simple           | Belle hero section sur l'accueil      |
| **3.2** | Section skills (Accueil)        | Liste des technos (hard-codée d'abord)                               | Grid de badges/chips avec les techs   |
| **3.3** | Page À propos - Texte           | Bio simple, infos basiques                                           | Page about lisible                    |
| **3.4** | Page À propos - Timeline        | Timeline du parcours (Epitech, expériences)                          | Timeline visuelle                     |
| **3.5** | Page Projets - Liste simple     | 3-4 projets hard-codés en tableau/grid                               | Liste des projets visible            |
| **3.6** | Carte projet (Card)             | Composant Card réutilisable (titre, desc, techs, liens)              | Cards bien présentées                 |
| **3.7** | Page projet détaillé            | Route `/projects/:id` → affiche un projet en détail                  | Clic sur projet = page détail         |
| **3.8** | Page Contact - Formulaire       | Form simple (nom, email, message) → log en console pour tester       | Formulaire fonctionnel (test en console) |
| **3.9** | Commit checkpoint               | `git add .` et `git commit`                                           | 📦 Portfolio complet mais sans animations |

---

### ✨ Phase 4 — Interactivité et animations

Ajouter du "wow" progressivement, seulement si ça teste bien.

| Étape   | Titre                      | Description                                                              | Résultat visible                          |
| ------- | -------------------------- | ------------------------------------------------------------------------ | ----------------------------------------- |
| **4.1** | Installer Framer Motion    | `npm install framer-motion`                                              | Rien encore (setup)                       |
| **4.2** | Animation hero au load     | Hero title fade + slide in au chargement                                 | Animation lisse au load                   |
| **4.3** | Animation skills au scroll | Les skills apparaissent au scroll (Intersection Observer ou Framer)       | Cards qui apparaissent au scroll           |
| **4.4** | Transition entre pages     | Fade out/in quand tu changes de page                                     | Pages qui transitionnent fluidement        |
| **4.5** | Hover effects              | Cards, boutons, liens avec hover animations                              | Feedback interactif en survol              |
| **4.6** | Easter egg optionnel        | Quelque chose de fun (Konami code, click secret, etc.)                   | Truc cool caché découvrable               |
| **4.7** | Commit checkpoint          | `git add .` et `git commit`                                              | 📦 Portfolio vivant et animé              |

---

### 🚀 Phase 5 — Production et polish

Optimiser avant le déploiement final.

| Étape   | Titre                      | Description                                                     | Résultat visible                 |
| ------- | -------------------------- | --------------------------------------------------------------- | -------------------------------- |
| **5.1** | Installer React Helmet     | `npm install react-helmet-async`                               | Rien encore (setup)              |
| **5.2** | SEO - Meta tags            | Title, description, Open Graph sur chaque page                  | Meta tags dans l'inspecteur      |
| **5.3** | Performance - Image lazy   | Images optimisées, lazy loading                                 | Chargement plus rapide           |
| **5.4** | Accessibility - ARIA       | ARIA labels, focus keyboard, alt text                           | Plus accessible aux lecteurs     |
| **5.5** | Setup GitHub Actions       | Créer workflow `.github/workflows/deploy.yml`                   | Déploiement auto sur GitHub      |
| **5.6** | Deploy en production       | `git push` → site live sur GitHub Pages ✨                     | 🚀 Portfolio en ligne !           |
| **5.7** | Commit final               | `git add .` et `git commit`                                     | 📦 Livré !                       |
