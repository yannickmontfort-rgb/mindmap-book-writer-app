# 📚 MindMap Book Writer

Logiciel d'écriture de livre basé sur une carte mentale : organisez vos parties, chapitres et scènes visuellement, puis rédigez directement dans l'application.

## 🧠 Comment ça marche

1. Créez un livre et choisissez son genre (roman, nouvelle, poésie, manuel pratique, mémoire).
2. Structurez-le sur la carte mentale : ajoutez des chapitres et des scènes, glissez-déposez pour réorganiser, renommez en un clic.
3. Basculez en mode Éditeur pour rédiger chaque scène en Markdown, avec aperçu en direct.
4. Exportez le livre entier en un clic quand il est prêt.

## ✨ Fonctionnalités

- 🗺️ **Carte mentale** interactive pour structurer votre livre (glisser-déposer, renommage rapide, raccourcis clavier)
- 🕐 **Chronologie de l'intrigue** : vue Gantt zoomable, calendrier personnalisable, événements liés aux personnages/lieux et aux scènes correspondantes
- 📚 **Multi-livres** : romans, nouvelles, poésie, manuels pratiques, mémoires — chacun avec sa structure et son vocabulaire adaptés (chapitres/scènes, poèmes, sections...)
- ✅ **Statut d'avancement** par chapitre/scène (Non commencé / En cours / Terminé)
- ✍️ Éditeur Markdown avec aperçu, objectifs de mots par scène/chapitre, minuteur Pomodoro, mode plein écran sans distraction, son de machine à écrire
- 🗂️ Fiches de référence (personnages, lieux, intrigue, sources...) en galerie de cartes, liées directement aux scènes concernées, avec photo (portrait pour les personnages, paysage pour les lieux)
- 🔍 Recherche plein texte dans tout le livre
- 🕐 Historique des versions par scène — rien n'est jamais perdu définitivement
- 📤 Export **Markdown**, **DOCX**, **PDF**, **PDF prêt pour Amazon KDP** (format 6x9", sommaire cliquable, mise en page adaptée à l'impression) et **EPUB** (liseuses, Kobo, Apple Books)
- 🌐 Disponible en **français et anglais**
- 💾 Sauvegarde automatique en continu

## ⬇️ Téléchargement (Windows)

👉 **[Télécharger le dernier installeur Windows](../../releases/latest)**

Application autonome (aucun prérequis .NET à installer séparément), avec choix du dossier d'installation et raccourcis Bureau/Menu Démarrer.

## 🐳 Version web / auto-hébergement (Docker)

MindMap Book Writer est aussi disponible en version web à auto-héberger (NAS, serveur Linux, PC toujours allumé...) — utile pour un usage multi-appareils : rédigez sur PC à la maison et continuez sur tablette en déplacement, avec les mêmes livres des deux côtés.

**Prérequis** : Docker + Docker Compose, ou un gestionnaire de conteneurs qui importe un `docker-compose.yml` (Portainer, Container Manager sur Synology DSM 7.2+).

1. Téléchargez [`docker-compose.yml`](docker-compose.yml)
2. `docker compose up -d` (ou import direct dans Portainer/Container Manager — aucun build requis, les images sont publiques)
3. Ouvrez `http://IP-DE-VOTRE-SERVEUR:5001` — un choix de langue (français/anglais) apparaît au premier lancement

**Sur un NAS Synology (DSM 7.2+)** : Container Manager → Projet → Créer → collez le contenu de `docker-compose.yml` → Suivant.

Vos livres sont stockés dans un volume nommé `mindmap-data`. Pour les stocker dans un dossier précis de votre NAS/serveur plutôt qu'un volume Docker anonyme, adaptez la section `volumes` du fichier (instructions en commentaire à l'intérieur).

## ☕ Soutenir le projet

Ce logiciel est gratuit et développé sur mon temps libre. Si vous l'appréciez et voulez soutenir son développement, un petit don est toujours apprécié :

👉 **[paypal.me/YMONTFORT](https://paypal.me/YMONTFORT)**

---

*Ce dépôt sert uniquement à la présentation et au téléchargement — le code source du projet est privé.*
