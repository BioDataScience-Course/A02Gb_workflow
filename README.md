# SDD I Module 2 : Workflow en biologie

## Avant-propos

Il est possible que ce document évolue au cours du temps. N'hésitez pas à aller vérifier le lien suivant afin de voir les modifications dans les consignes : <https://github.com/BioDataScience-Course/A02Gb_workflow>

## Objectif

Ce projet est un projet **individuel**, **court** et **cadré** qui doit être terminé pour la fin du module 2. Il porte sur la biométrie humaine. Son but est de vous faire réaliser l'intérêt de R Markdown pour écrire des documents scientifiques de manière à ce qu'ils soient reproductibles et faciles à mettre à jour.

## Consignes

Vous êtes dans la peau d'un biologiste qui analyse des données de biométrie humaine. Vous avez à votre disposition deux jeux de données répartis en deux fichiers, disponibles à partir du sous-dossier `data` de ce projet.

- `biometry_2014.xlsx`
- `biometry_2016.xlsx`

Ces fichiers comprennent 7 variables :

- gender : homme (H) ou femme (F)
- db : date de naissance
- yb : année de naissance
- weight : masse en kg
- height : taille en cm
- wrist : circomférence du poignet en mm
- measurement_date : année de la prise de mesure

#### Analyse de `biometry_2014.xlsx`

- Utilisez ce jeu de données afin de réaliser un graphique de type nuage de points (choisissez-en un qui vous parait pertinent). Pour cela, utilisez le script R `biometry_graphe.R` qui est dans le sous-dossier `R`.

- Incorporez ensuite le graphique généré dans un rapport sous Microsoft Word (fichier nommé `biometry_word.docx` et placé dans le sous-dossier `docs`). Structurez votre rapport avec les différentes sections de la rédaction scientifique (introduction, but, matériel et méthodes, résultats, discussion et conclusions). Ajoutez une courte phrase relative à chaque section pour donner un peu de contenu à votre rapport, sans plus. Le graphique est à incorporer dans la section "résultats". Des explications détaillées sur la rédaction scientifique se trouvent dans l’[annexe ](https://wp.sciviews.org/sdd-umons/?iframe=wp.sciviews.org/sdd-umons-2020/redaction-scientifique.html) dédiée à cette dernière.

- Réalisez ensuite le même rapport mais dans un document R Markdown (format .Rmd). Pour cela, complétez le document `biometry.Rmd` mis à votre disposition dans le sous-dossier `docs` avec les différentes sections propre à un rapport scientifique. Copiez-y le texte que vous avez écrit précédemment, et utilisez le formattage propre à markdown. Incorporez-y également le graphique de type nuage de point dans la partie "résultats". Pour cela, copiez le code R issu du script `biometry_graphe.R` dans un chunks permettant de lire les données, et ensuite de réaliser le graphique.

- Compilez votre rapport R Markdown en trois formats différents : "HTML", "PDF" et "Word". Examinez le résultat, et comparez en particulier les deux version Word de votre rapport.

- Réalisez un `commit` signifiant la fin de cette première analyse. 

### Nouvelles données `biometry_2016.xlsx`

Après avoir réalisé une première version de vos rapports, l'un dans Word, et l'autre dans R Markdown, avec les données de `data/biometry_2014.xlsx`, vous recevez de nouvelles données (celles dans`data/biometry_2016.xlsx`).

- Actualisez votre rapport sous Microsoft Word avec ces nouvelles données. Vous devez bien évidemment actualiser le graphique, ce qui revient donc à remplacer l'ancienne version par un graphique recalculé avec toutes les données 2014 + 2016.

- Faites de même pour votre rapport sous R Markdown.

### Comparaison des deux méthodes

A la suite de vos analyses, répondez aux questions ci-dessous pour cadrer votre réflexion sur le workflow et la recherche reproductible.

Utilisez un fichier RMarkdown (`.Rmd`) pour y consigner vos réponses et placez-le dans votre projet RStudio. Nommez ce fichier `workflow.Rmd`

- Quel workflow vous semble le plus simple à l'utilisation, et pourquoi ?

- Comparez la façon dont les graphiques sont gérés dans les deux cas.

- Quel workflow vous semble le plus pertinent lorsque les données arrivent progressivement ?

- Quel workflow vous semble le plus simple et le plus approprié lorsque plusieurs personnes collaborent pour rédiger un rapport ? 

### Etat de progression 

A la fin de ce module, vous devez avoir :

- un script R nommé `biometry_graphe.R` (dans le dossier `R`) qui comprend vos premiers graphique que vous utiliserez dans le document `biometry_word.docx` (dans le dossier `docs`)

- un fichier au format .doc ou .docx nommé `biometry_word.docx` (dans le dossier `docs`) comprend le nuage de point le plus à jour.

- un fichier au format .Rmd nommé `biometry.Rmd` (dans le dossier `docs`) qui comprend le nuage de point le plus à jour.

- un fichier au format .Rmd nommé `workflow.Rmd` (dans le dossier `docs`) qui comprend votre comparaison des workflows.
