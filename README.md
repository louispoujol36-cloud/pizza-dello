# Pizza Dello — pizzadello.fr

Site vitrine de la pizzeria Pizza Dello (Taller, Landes). Une seule page statique, hébergée sur GitHub Pages.

## Fichiers

| Fichier | Rôle |
|---|---|
| `index.html` | Tout le site : contenu, styles et script |
| `404.html` | Page affichée pour une adresse inconnue |
| `images/`, `fonts/` | Photo de la façade et polices (hébergées ici, aucun service externe) |
| `favicon.png`, `favicon.svg` | Icône du site |
| `CNAME` | Nom de domaine utilisé par GitHub Pages — ne pas supprimer |
| `sitemap.xml`, `robots.txt` | Pour les moteurs de recherche |

## Modifier le site

- **Un prix ou un plat** : dans `index.html`, chercher le nom du plat.
- **Les horaires**, à deux endroits dans `index.html` :
  1. le tableau `id="horaires"` : le texte affiché **et** les attributs `data-ouvre` / `data-ferme`
     (le message « Ouvert / Fermé » en haut de page est calculé à partir de ces attributs ; une ligne sans attributs = jour fermé) ;
  2. `openingHoursSpecification` en haut du fichier (lu par Google).
- **L'étiquette « Nouveau »** : retirer `nouveau` de la classe du plat et le `<span class="badge badge-nouveau">`.

Mise en ligne : un `git push` sur la branche `main` suffit, le site est à jour en une à deux minutes.

## Services externes

- **GoatCounter** (statistiques sans cookies) : https://popix.goatcounter.com
- **Google Maps** : plan intégré dans la partie « Où nous trouver ? »
- **OVH** : nom de domaine `pizzadello.fr` (zone DNS pointant vers GitHub Pages)
