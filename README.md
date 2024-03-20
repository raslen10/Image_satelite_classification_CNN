# Image_satelite_classification_CNN
Classification d'images satellites avec CNN 

Ce projet vise à classifier des images satellites en utilisant un réseau de neurones convolutionnel (CNN). Les images satellites sont des données multispectrales, chaque pixel contenant des informations provenant de différentes bandes spectrales (rouge, vert, bleu et infrarouge). 
L'objectif est de prédire la catégorie à laquelle appartient chaque image, parmi quatre classes : Terrain stérile, Arbres, Terrain herbeux et Autre. 

Étapes suivies : 
Prétraitement des données : Les images satellites ont été prétraitées pour les mettre dans un format approprié pour l'entraînement du CNN. Cela comprend le chargement des données à partir de fichiers CSV, le redimensionnement des images en 28x28 pixels avec 4 canaux, et la normalisation des valeurs de pixel entre 0 et 1. 
Construction du modèle CNN : Un modèle CNN simple a été construit en utilisant TensorFlow. Le modèle comprend plusieurs couches de convolution et de pooling, suivies de couches entièrement connectées. La fonction d'activation ReLU est utilisée pour les couches cachées, tandis que la couche de sortie utilise une fonction d'activation softmax pour la classification multiclasses. 
Entraînement du modèle : Le modèle CNN a été entraîné sur un ensemble de données d'entraînement à l'aide de l'algorithme de descente de gradient stochastique avec la fonction de perte de cross-entropy catégorique. L'optimiseur Adam a été utilisé pour minimiser la perte. 
Évaluation du modèle : Le modèle entraîné a été évalué sur un ensemble de données de test pour évaluer sa performance. Les mesures d'évaluation comprennent la précision (accuracy) et la perte (loss) obtenues sur l'ensemble de test. 

Résultats : Après l'entraînement du modèle CNN, 
les performances suivantes ont été obtenues sur l'ensemble de test : Précision : 97% Perte : 0.08 

Le modèle a montré une précision élevée dans la classification des images satellites, démontrant ainsi son efficacité dans ce domaine.
