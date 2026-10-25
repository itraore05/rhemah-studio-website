# 🎙️ Rhemah Studio — Site vitrine d'un studio de production musicale à Londres

![Next.js](https://img.shields.io/badge/Next.js-16-000000?style=flat&logo=nextdotjs&logoColor=white)
![React](https://img.shields.io/badge/React-19-61DAFB?style=flat&logo=react&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-5-3178C6?style=flat&logo=typescript&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind%20CSS-4-06B6D4?style=flat&logo=tailwindcss&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=flat&logo=vercel&logoColor=white)
![Statut](https://img.shields.io/badge/statut-en%20ligne-success?style=flat)

> Site vitrine **bilingue (FR / EN)** de Rhemah Studio Ltd, studio d'enregistrement, de production musicale et de podcast basé à **Londres**, qui rassemble et accompagne les talents de la communauté francophone d'Afrique.
> **Projet client** (2026) — conception et développement de bout en bout.

🔗 **Site en ligne : [rhemah-studios.vercel.app](https://rhemah-studios.vercel.app/fr)**

> ℹ️ Dépôt vitrine : le code source appartient au client et reste privé. Cette page présente le projet, les choix techniques et mon travail.

---

## 🎯 Le besoin du client

Le fondateur, musicien professionnel, voulait un site qui :

- donne de la **visibilité** au studio et installe une **réputation professionnelle** ;
- fédère une **communauté francophone** de musiciens à Londres ;
- permette de **réserver une session** ou de **demander un devis** facilement ;
- respecte le **UK GDPR**, puisque le studio est une société britannique.

Le projet suit un **cahier des charges** validé avec le client, puis une validation de l'interface page par page.

## ✨ Ce que fait le site

- **7 pages**, chacune en français et en anglais : accueil, à propos, services, réservation, contact, mentions légales, confidentialité
- **Détection automatique de la langue** du navigateur et sélecteur FR / EN qui conserve la page en cours
- **Bannière d'accueil animée** : les 5 barres du logo deviennent des photos du studio et montent comme un égaliseur
- **Formulaires de contact et de réservation** : validation côté serveur, anti-spam, consentement, envoi par e-mail
- **Réservation en ligne** avec Calendly, chargé seulement au clic
- **Services** avec aperçu photo au survol et bouton « Réserver » qui présélectionne le service
- **Vidéos YouTube** chargées au clic, en mode sans cookie

## 🛠️ Stack technique

| Besoin | Outil |
|---|---|
| Framework | Next.js 16 (App Router, Server Actions, Cache Components) |
| Interface | React 19, TypeScript 5 |
| Styles | Tailwind CSS 4, thème sur mesure |
| Langues | i18n native de Next.js, dictionnaires typés (aucune librairie) |
| Formulaires | Server Actions + validation zod |
| E-mails | Resend |
| Réservation | Calendly |
| Statistiques | Vercel Analytics (sans cookie) |
| Hébergement | Vercel (déploiement continu depuis GitHub) |

## 🧩 Choix techniques marquants

- **Traductions typées** : le dictionnaire anglais est typé sur le français. Une clé oubliée fait échouer le build, donc aucune page ne peut partir en ligne à moitié traduite.
- **Pages 100 % statiques** : pas de base de données en V1, donc un site rapide, peu coûteux et sûr.
- **Formulaires sécurisés** : validation côté serveur, champ piège contre les robots, e-mails en texte brut (pas d'injection HTML).
- **Vie privée dès la conception** : aucun cookie non essentiel. YouTube et Calendly ne se chargent qu'au clic, d'où l'absence de bannière cookies.
- **SEO** : métadonnées par page et par langue, balises `hreflang`, Open Graph, sitemap et robots.txt générés automatiquement.
- **Accessibilité** : focus clavier visible, lien « Aller au contenu », animations désactivées si l'utilisateur le demande.
- **Images optimisées** : `next/image`, formats modernes, tailles adaptées à chaque écran, aperçu flou au chargement.

## 🎨 Identité visuelle

Le design s'appuie sur le logo « 5.RHEMAH STUDIOS » et ses **5 barres verticales**, reprises dans la bannière, les photos et le favicon. Palette bordeaux et or, une seule police (Montserrat, celle du logo), de vraies photos du studio plutôt que des images de banque.

## 🗺️ Évolutions prévues (V2)

- Portfolio audio et vidéo des productions
- Espace communauté : annuaire des artistes, agenda des événements
- Blog et newsletter
- Back-office avec **Payload CMS**, intégré à l'application Next.js

## 💡 Compétences démontrées

- Relation client : cahier des charges, validation par étapes, livraison
- Développement **Next.js / React / TypeScript** moderne
- Site **multilingue** et **SEO international**
- Conformité **UK GDPR** et respect de la vie privée
- Déploiement continu sur **Vercel**

## 👤 Auteur

**Ismaël Traoré** — Développeur Data & IA
📧 contact.traoreimael@gmail.com · 💼 [LinkedIn](https://www.linkedin.com/in/ismael-traor%C3%A9-m-4007a2225/)
