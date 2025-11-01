# ThinkIA — Jekyll starter (GitHub Pages friendly)

Un site simple et moderne pour publier des articles quotidiens.
- Accueil : 2–3 derniers articles
- Lien vers les 20 derniers
- Menu latéral : thèmes (catégories) + compte d'articles, clic = page du thème

## Déploiement rapide (GitHub Pages)
1. Créez un dépôt **thinkia-site** sur GitHub et poussez ces fichiers.
2. Dans *Settings ▸ Pages*, sélectionnez la branche `main`, dossier `/root`.
3. Publiez vos articles dans `_posts/` au format `YYYY-MM-DD-titre.md`.

## Écriture d’un article
Exemple minimal :
```markdown
---
title: "L'IA et l'emploi : signaux contrastés"
description: "Analyse rapide des dernières annonces et publications."
categories: [Actualité, Société]
tags: [IA, emploi, économie]
---

Votre contenu en **Markdown**…
```