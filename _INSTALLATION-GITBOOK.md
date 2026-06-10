# 📦 Guide d'installation — Wiki Horizon RP sur GitBook

Ce dossier est un **wiki GitBook complet, prêt à publier**. Voici comment le mettre en ligne. Tu as **deux méthodes** : Git Sync (recommandé, pro) ou import manuel.

> ℹ️ Ce fichier (`_INSTALLATION-GITBOOK.md`) est une **notice pour toi**, il n'apparaîtra pas dans le wiki (il n'est pas dans le `SUMMARY.md`).

---

## ✅ Méthode 1 — GitHub + GitBook Git Sync (recommandée)

C'est la méthode la plus propre : ton wiki vit sur GitHub et se synchronise tout seul avec GitBook.

### Étape 1 — Créer un dépôt GitHub

1. Crée un compte sur [github.com](https://github.com) si besoin.
2. Crée un **nouveau dépôt** (ex : `astra-rp-wiki`), en **privé** ou public.

### Étape 2 — Envoyer ces fichiers sur GitHub

Depuis ce dossier (`astra-rp-wiki`), en ligne de commande :

```bash
git init
git add .
git commit -m "Wiki Horizon RP - version initiale"
git branch -M main
git remote add origin https://github.com/TON-PSEUDO/astra-rp-wiki.git
git push -u origin main
```

> 💡 Pas à l'aise avec Git ? Tu peux aussi **glisser-déposer** tous les fichiers et dossiers directement sur la page du dépôt GitHub via le bouton **« Add file → Upload files »**. Pense à bien garder l'arborescence (dossiers `reglement/`, `guide/`, `.gitbook/`, etc.).

### Étape 3 — Connecter GitBook

1. Va sur [gitbook.com](https://www.gitbook.com) et connecte-toi.
2. Crée un **nouvel espace** (Space).
3. Dans **Settings → Integrations → Git Sync**, connecte ton **GitHub**.
4. Sélectionne le dépôt `astra-rp-wiki` et la branche `main`.
5. Choisis le sens **GitHub → GitBook**.
6. Lance la synchro : **tout le wiki apparaît automatiquement** avec la navigation. 🎉

---

## ✅ Méthode 2 — Import manuel rapide (sans GitHub)

Si tu veux juste tester vite :

1. Sur GitBook, crée un **espace**.
2. Recrée la structure des pages en suivant le `SUMMARY.md`.
3. **Copie-colle** le contenu de chaque fichier `.md` dans la page correspondante.
4. **Uploade les images** du dossier `.gitbook/assets/` dans GitBook (glisser-déposer dans chaque page).

> ⚠️ Cette méthode est plus longue et manuelle. La **Méthode 1 (Git Sync)** est vraiment recommandée.

---

## 🗂️ Structure du wiki

```
astra-rp-wiki/
├── .gitbook.yaml          ← config GitBook (ne pas supprimer)
├── README.md              ← page d'accueil
├── SUMMARY.md             ← le sommaire / la navigation
├── .gitbook/assets/       ← toutes les images (bannières, logo, VIP…)
├── informations/          ← Lore, Lexique
├── guide/                 ← Connexion, touches, emploi
├── reglement/
│   ├── general/           ← Règles de base, zones
│   ├── services-publics/  ← SASP, SAMS, DEFCON, entreprises
│   └── illegal/           ← Gangs, MC, indépendants
├── boutique/              ← VIP, achat, remboursement
├── support/               ← Support, modération, report
└── bugs/                  ← Cache, fichiers, bug de map
```

---

## ✏️ Personnaliser ton wiki

Tout est éditable ! Pense notamment à remplacer les **valeurs à compléter** :

- [ ] `discord.gg/astrarp` → ton **vrai lien Discord** (dans plusieurs pages).
- [ ] `astra-rp.tebex.io` → ta **vraie boutique** (pages boutique).
- [ ] `cfx.re/join/xxxxxx` → ton **lien de connexion FiveM** (page connexion).
- [ ] Les **grades, prix VIP, DEFCON et procédures** → adapte-les à TON serveur.
- [ ] Les **noms de zones safe/gunfight** → mets tes zones réelles.

> 🔎 Astuce : fais une recherche sur `xxxxxx`, `astrarp` et `tebex` dans tous les fichiers pour trouver rapidement ce qui est à remplacer.

---

## 🎨 Conseils GitBook pour un rendu pro

- Active un **thème sombre** dans GitBook (Customization) pour coller à l'identité bleu cyan / noir d'Horizon.
- Mets le **logo** (`.gitbook/assets/logo.png`) en icône de l'espace (Settings → Customization).
- Définis une **couleur d'accent bleu cyan** pour rappeler tes bannières.
- Active la **recherche** et le **sommaire de page** (déjà prévus dans la config).

---

Bon courage et bon lancement pour **Horizon RP** ! 🌅
