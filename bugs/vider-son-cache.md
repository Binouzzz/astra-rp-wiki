---
description: Nettoyer le cache de FiveM pour régler crashs, lags et bugs de texture.
---

# 🧹 Vider son cache

<figure><img src="../.gitbook/assets/banner-vider-cache.png" alt="Vider son cache"><figcaption></figcaption></figure>

Vider le **cache de FiveM** est la solution n°1 pour la plupart des problèmes : crashs, lags, textures buguées, chargement infini ou ressources qui ne se mettent pas à jour.

{% hint style="info" %}
Vider le cache **ne supprime rien d'important** : FiveM le reconstruit automatiquement à la prochaine connexion (le premier chargement sera juste un peu plus long).
{% endhint %}

***

## 🧹 Méthode 1 — Le cache FiveM (recommandée)

1. **Ferme complètement FiveM.**
2. Ouvre l'**Explorateur de fichiers** Windows.
3. Dans la barre d'adresse, colle :
   ```
   %localappdata%\FiveM\FiveM.app\data
   ```
4. Ouvre le dossier **`cache`**.
5. **Supprime tout** son contenu **SAUF** le dossier/fichier **`servers`** et **`game-storage`** si présents.

{% hint style="warning" %}
**Ne supprime PAS** le dossier `priv` ni tes fichiers de licence. Vide uniquement le contenu du dossier **`cache`** (hors `servers`).
{% endhint %}

***

## 🧨 Méthode 2 — Cache complet (si ça persiste)

Si le problème continue :

1. FiveM fermé, va dans :
   ```
   %localappdata%\FiveM\FiveM.app\data
   ```
2. Supprime entièrement les dossiers **`cache`** et **`server-cache`**.
3. Relance FiveM et reconnecte-toi (le téléchargement initial repartira de zéro).

***

## ⚙️ Méthode 3 — Cache GTA (textures/streaming)

Pour les bugs de **textures et de streaming** :

1. Va dans :
   ```
   %localappdata%\FiveM\FiveM.app\citizen
   ```
2. Recherche les caches liés au streaming/texture et nettoie-les.
3. En dernier recours, une **réinstallation propre** de FiveM règle les cas extrêmes.

***

## ✅ Après avoir vidé le cache

* 🔄 **Relance** FiveM.
* ⏳ Le **premier chargement** sera plus long (re-téléchargement) : c'est normal.
* 🎮 Reconnecte-toi à **Astra RP**.

{% hint style="success" %}
Toujours un souci ? Tente la [vérification des fichiers GTA V](verifier-fichiers.md), puis ouvre un ticket sur le [Support](../support/support.md) si nécessaire.
{% endhint %}
