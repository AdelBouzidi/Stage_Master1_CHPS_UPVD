# Stage_Master1_CHPS_UPVD
Mise en Place d'un Cluster Kubernetes et Déploiement d’un Pipeline MLOps LSTM sur le Cluster avec Techniques d’Optimisation HPC

Le système MLOps mis en place dans le cadre de ce stage permet d’automatiser et d’orchestrer l’ensemble du cycle de vie d’un modèle LSTM pour l’autocomplétion de texte, avec une mise à jour périodique des données d’entraînement et une regénération continue des modèles entrainées.

le pipeline comprend les étapes suivantes : 
1) la mise à jour périodique des données d'entraînement en ajoutant régulièrement de nouvelles phrases aux données d'entraînement, ces phrases sont générées via un programme,
2) l'entraînement du modèle LSTM séquentiel et distribué,
3) l’évaluation continue des modèles LSTM entraînés (séquentiel et distribué), à travers l’exposition de métriques mesurant le pourcentage de prédictions correctes via Prometheus, permettant une visualisation comparative dans le navigateur.
4) démonstration de la prédiction via :
   a) une interface web statique affichant des résultats pré-calculés,
   b) une interface web interactive permettant à l’utilisateur de tester directement la prédiction.
Les fichiers présents dans ce répositorie décrit en détail le rôle et le fonctionnement des principaux composants et modules. 
