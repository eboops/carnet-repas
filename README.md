# Carnet de repas

Un carnet de suivi alimentaire **simple et sans compte** : on note ce qu'on mange, le carnet calcule les calories et les protéines.

Prototype en HTML d'une future application Android (Kotlin, Jetpack Compose).

## Principes

- **Pas de compte, pas de serveur** : les données restent dans le navigateur de l'appareil.
- **Valeurs crues pour 100 g**, prises sur les emballages ; on pèse avant cuisson.
- **Portions nommées** (« tranche », « pot », « cuillère à café ») et fractions (0,5 ou 0,33 portion).
- **Une petite base d'aliments courants** (table Ciqual de l'ANSES), classés par catégories, modifiables et supprimables.
- **L'analyse est confiée à une IA** : le bouton « Copier pour une analyse » produit un texte détaillé, jour par jour et repas par repas, à coller dans une conversation.

## Écrans

1. **Aliments** : nom, catégorie, kcal et protéines pour 100 g, portion habituelle et son nom.
2. **Repas** : date, heure, type de repas, aliments en grammes ou en portions ; modification d'un repas enregistré ; le repas en cours est conservé.
3. **Bilan** : jour (jauges par rapport aux objectifs) ou semaine (graphique), objectifs quotidiens, analyse, sauvegarde et restauration.

## Sauvegarde et changement d'appareil

Les données de chaque appareil sont indépendantes. Pour passer d'un appareil à l'autre :

1. sur l'ancien : **Bilan → Enregistrer dans un fichier** (ou « Copier la sauvegarde complète ») ;
2. sur le nouveau : **Bilan → Restaurer une sauvegarde**, puis vérifier le résumé (date, appareil, nombre d'aliments et de repas) avant de confirmer.

## Publication avec GitHub Pages

Déposer `index.html` à la racine du dépôt, puis **Settings → Pages → Deploy from a branch → main / (root)**.
