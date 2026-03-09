PROJET TUTORE :
Prédiction du taux de criminalité à l'aide de K moyennes.

                               Contexte du projet :
 Les villes souhaitent analyser et anticiper les zones à forte criminalité afin d'améliorer la sécurité. L’analyse des données permet d’identifier les zones à risque et les tendances criminelles. Dans ce projet, l’algorithme K moyennes (K means) est utilisé pour regrouper les zones selon leur niveau de criminalité

1-Objectif du logiciel:

Le logiciel doit permettre à une autorité (police, municipalité, analyste) de prévoir et analyser le taux de criminalité dans une zone donnée afin de :
	-Identifier les zones à risque.
	-Détecter des motifs récurrents de criminalité (heure, lieu, type de crime).
              -Regrouper les crimes et les criminels en clusters pour des analyses ciblées.
	-Aider à la prise de décisions pour la sécurité publique (renforcement policier, prévention).

2-Besoins fonctionnels détaillés:

2.1 Gestion des données:
	-Saisie des données criminelles par un administrateur:
	-Lieu du crime (latitude/longitude, quartier, ville).
	-Type de crime (vol, agression, trafic…).
	-Heure et date du crime.
	-Gang ou groupe criminel impliqué (si connu).
	-Importation de fichiers CSV ou bases de données externes.
	-Validation et nettoyage automatique des données : pas de doublons, format standardisé.

2.2 Analyse des données:
	-Application de l’algorithme K-means pour regrouper les crimes en clusters selon :
	-Localisation géographique.
	-Type et heure du crime.
	-Détection des zones à forte criminalité.
	-Possibilité de paramétrer le nombre de clusters k.

2.3 Visualisation et rapports:
	-Cartes interactives montrant les clusters de crimes.
	-Graphiques statistiques (histogrammes, diagrammes en barres ou heatmaps).
	-Rapports exportables (PDF, Excel) pour présentation aux autorités.

2.4 Utilisateurs et accès:
	-Administrateur : saisie et gestion des données, paramétrage des analyses.
	-Analyste / Autorité : consultation des clusters et des visualisations.
	-Gestion des droits d’accès pour protéger les données sensibles.
3- Besoins non fonctionnels:
	-Performance : traitement efficace même avec de grandes quantités de données (ex : 100 000 crimes/an).
	-Sécurité : chiffrement des données sensibles, authentification des utilisateurs, journalisation des accès.
	-Fiabilité et précision : les clusters doivent refléter la réalité du terrain pour que les décisions soient pertinentes.
	-Extensibilité : ajouter facilement de nouvelles zones ou de nouveaux types de crimes.
	-Interopérabilité : possibilité d’importer/exporter les données avec d’autres systèmes policiers ou bases publiques.
	-Facilité d’utilisation : interface claire pour utilisateurs non techniques.
4-Contraintes du projet:
	1.Données :
 la qualité des prédictions dépend des données disponibles (ex : absence ou inexactitude des données peut fausser les clusters).
	2.Confidentialité : 
respecter la législation sur les données personnelles et criminelles.
	3.Infrastructure : 
le logiciel doit pouvoir fonctionner sur des serveurs existants ou cloud.
	4.Maintenance : 
mise à jour régulière des données et de l’algorithme pour garder les prédictions pertinentes.
	5.Technologie :
 le choix des langages et bibliothèques (Python, scikit-learn, bases SQL, outils de visualisation) doit être compatible avec les ressources disponibles.
