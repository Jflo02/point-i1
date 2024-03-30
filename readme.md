# Guide d'installation de l'environnement de développement

Ce guide vous aidera à installer NVIDIA CUDA Toolkit et à lancer le projet xtts sur votre ordinateur

## Étape 1: Télécharger NVIDIA CUDA Toolkit

Téléchargez le [NVIDIA CUDA Toolkit](https://developer.nvidia.com/cuda-toolkit) sur votre PC Windows.

## Étape 2: Installer Docker

Assurez-vous d'avoir Docker installé en utilisant WSL 2. Vous pouvez suivre ce [guide d'installation de Docker](https://docs.docker.com/docker-for-windows/wsl/).

## Étape 3: Lancer Docker Desktop

Lancez le conteneur à l'aide du fichier docker-compose.yaml

Un jupyter notebook a été lancé sur le port 8888 de votre machine.
Veuillez vous y connecter en utilisant le token qui apparait dans les logs du conteneur

## Étape 4: Vérification

Chaque bout de code devrait se lancer sans problème. Le deuxième code block devrait indiquer "cuda". Si "cpu" est affiché cela signifie qu'il y a à un problème avec le setup de cuda et que le modèle tourne sur le cpu et non pas le gpu.

Vérifiez que tout fonctionne correctement. Si vous rencontrez des problèmes, consultez la [documentation officielle de Docker](https://docs.docker.com/get-started/overview/) ou la [documentation de NVIDIA CUDA Toolkit](https://docs.nvidia.com/cuda/).