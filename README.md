# Saisie de commande — maquette de LVA Distribution

Proposition d'ergonomie pour l'écran de saisie de commande client d'Hélios Cloud.

- Note d'introduction : <https://lva-distribution.github.io/lva-maquettes/>
- Maquette : <https://lva-distribution.github.io/lva-maquettes/saisie-b/>

Une ébauche, pas un logiciel : elle sert de cahier des charges qu’on peut cliquer. Le code et les idées peuvent être repris librement pour Hélios.

## Contenu

| Fichier | Rôle |
| --- | --- |
| `index.html` | note d'introduction |
| `saisie-b/index.html` | la maquette, en une seule page (HTML, CSS et JavaScript, sans bibliothèque) |
| `saisie-b/photos/` | photos des articles, nommées par code article |

## Lire `saisie-b/index.html`

Le fichier se lit de haut en bas, chaque bloc commence par un commentaire `// ----- titre` :

1. **Styles** : couleurs en variables CSS en tête ; vert pastel des lignes saisies, alternance ton sur ton, + / − au survol (`.qbox`), vignettes d'historique et pulsation (`.histo`, `.clign`).
2. **Données** : `A` = cadencier du client (article, unités, tarif, 5 semaines d'historique, stock, colisages proposés) ; `CATALOGUE` = tout le catalogue pour la recherche F3. Client fictif, prix et historiques inventés.
3. **Calculs** : colisage choisi et conversion vers l'unité de prix, prix d'une unité de commande, total de ligne, remise par rapport au tarif général, quantité habituelle.
4. **Dessin** : volet client, filtres, cadencier par familles repliables, volet commande.
5. **Clavier** : barre F2 (articles du client) et F3 (catalogue), Entrée, flèches, raccourcis `2c` / `3p`.
6. **Prix** : bulle remise % ou prix net, nature TG / CP / TS.
7. **Bandeau** : fiche client (livraisons, factures, tournées), calendrier de livraison, devis / commande.
8. **Mode devis** : colonne de remises à la chaîne, enregistrement groupé.

Rien n'est envoyé nulle part : la page n'appelle aucun serveur.
