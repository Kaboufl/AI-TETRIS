# Initial prompt

Crée un jeu Tetris en HTML, CSS et JavaScript, jouable par deux joueurs : un humain et une intelligence artificielle (IA). Le jeu doit comprendre les fonctionnalités suivantes :

**Interface et Grilles :**

* Deux grilles de jeu distinctes, affichées côte à côte : une pour le joueur humain et une pour l'IA.
* Un tableau des scores clair, affichant les points en temps réel pour chaque joueur.

**Joueur Humain :**

* Contrôles intuitifs via les flèches du clavier : gauche, droite, bas pour déplacer les pièces, haut pour les faire pivoter.

**Intelligence Artificielle (IA) :**

* L'IA joue automatiquement, en utilisant une logique simple pour placer les pièces de manière efficace.

**Système de Score :**

* 50 points par ligne complétée.
* Bonus de 100, 200 et 300 points pour 2, 3 et 4 lignes complétées simultanément (Tetris).

**Règles Spéciales et Bonus :**

* "Cadeau surprise" : Lorsqu'un joueur fait 2 lignes en un coup, l'adversaire reçoit une pièce facile (carré ou ligne).
* "Pause douceur" : Tous les 1000 points, les pièces ralentissent de 20% pendant 10 secondes.
* "Pièce rigolote" : Tous les 3000 points, une pièce spéciale (cœur, étoile) apparaît, valant 100 points bonus.
* "Échange amical" : Un Tetris permet d'échanger une ligne pleine avec une ligne vide de l'adversaire.
* "Arc-en-ciel" : Toutes les 2 minutes, les couleurs des pièces changent pendant 20 secondes.

**Conseils Techniques :**

* Utilise <canvas> ou des grilles de <div> pour les terrains de jeu.
* Crée des animations CSS pour la disparition des lignes.
* Gère les grilles avec des tableaux 2D en JavaScript.
* Implémente un timer pour gérer les règles temporaires.

**Objectif :**

* Crée un jeu Tetris compétitif et amusant, où l'IA et l'humain peuvent s'affronter dans une ambiance conviviale. Le tableau des scores doit clairement indiquer le gagnant.

# Prompts used in copilot

Considering the following tetris logic, refactor the computeBestMove function to enhance the AI behavior

Add a timeout to slow down the AI in its gameplay logic

Now each time the player clears a line, the AI delay gets reduced until a floor of 15ms

Redesign the tetris user interface to be more friendly