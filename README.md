# wine-label 

Le but ici est de faire en sorte que l'ordinateur puisse lire l'étiquette d'une bouteille de vin à partir d'une simple photo. Pourquoi est-ce compliqué, vous demandez-vous peut-être ? Eh bien, tout d'abord, nous ne pouvons pas appeler directement une bibliothèque OCR (reconnaissance optique de caractères) comme Tesseract, car le texte sur l'étiquette est déformé sur un cylindre et nous ne pouvons pas extraire correctement les caractères et donc les mots et les phrases.

Pour utiliser ce package sur votre machine, vous devez installer les dépendances du fichier requirement.txt, déplacer la photo que vous souhaitez utiliser pour l'entraînement dans le dossier "X" et les masques dans le dossier "y", et la photo que vous souhaitez lire dans le dossier "to_read". Pour configurer l'emplacement des fichiers ou les paramètres du U-Net, utilisez le fichier Config.json.

## train model on images
```
python main.py --train
```
## read images
```
python main.py --read
```
## train then read images
```
python main.py --train --read
```
