Finalement,  README.txt  sera ma deuxième modification. Pour insérer des caractères avec VIM c'est "A". Pour quittervim, la commande est :wq
Je commence à apprécier utiliser le terminal. Fort bien, continuons.

Présentons le projet: Comment GIT et GITHUB fonctionne

Git init tu feras en premier, git status tu suivras.
Git init permet de reinitialiser ou d'initialiser Git sur un repository.
Il est important de le faire au tout début de notre tâche sur Git.
1) Git init, mkdir xxx, cd xxx, git  status, git  init, git status, touch  checklist, git add  checklist, git status,  git commit  -m, git status : voici un peu le  cheminement à réaliser pour lancer un  nouveau  DOSSIER  sur lequel  nous allons travailler

Avec cette suite de commande (ci-dessus), nous venons d'initialiser notre répertoire Git,et nous créons un dossier pricipal. J'entre dans le dossier créé. Je vérifie le status de Git sur mon  nouveau  dossier. Je reinistialise Git  sur le terminal pour l'informer que ce sera le dossier "maître" (Git observera et nous notifiera de tout changement). Bien entendu, je vérifie le status à nouveau, car il suit la commande "git init". Enfin je décide de créer un fichier .md pour commencer un projet (touch checklist), et les commandes "git-add" et "git commit -m" afin de l'ajouter à l'index sur Git (tracabilité du projet). On fini par 'git status' pour vérifier si toute action a été commit (commenter) par l'auteur.

Dans une première phase de ce cours + projet : on apprend à créer un dossier à partir de notre terminal, où nous allons enregistrer des documents grâce au logiciel de Git, celui-ci  nous permettant  de  faire  des  sauvegardes  lorsqu'on travaille sur un projet.
Donc on  créer un dossier  (mkdir) et on entre (cd) et enfin on créer un fichier que nous souhaitons (.md, .txt,  etc.)
Pour afficher  la  liste des fichiers présents dans un dossier choisi (HEAD) nous réalisons la commande "ls"

Toutes les modifications réalisées sur le code  d'un fichier  doit se suivre 0) git status  1) d'un  git add avec le nom du fichiermodifié 2)d'un git  commit  - m : permettant de décrire ce qui a été réalisé sur la modification, ou l'ajout ou la  supression  d'un fichier. Soit nous avons en raccourci après la modification d'un document : a) git status et  suivi d'un git commit -am "description du changement/création". Lui permet de "add toute modifications et de commit un Message -m à la fois".

le  commit est super, car il nous permet dans u 1er temps  d'avoir l'auteur, son SHA (unique par commit), la  date de modification. celui ci est  très utile afin de garder une trace  de son évolution lorsqu'on construit son code. Git nous permet de sauvegarder une version de notre projet/ code à un instant T. iL nous permet de remonter dans le temps si notre code commence à bugger. Nous pouvons mieux remonter les différentes phases de conception et d'identifier à partir de quand le bug à pu surgir.

Git range les modifications dans l'index créer au tout début. 

Lorsqu'on travail à plusieurs, nous devons fréquemment  réalisées des commits (git commit -m ou -am) et des gits pushs (git  push origin master) et des git pulls (git pull origin master). PUSH pour qu'ON envoi nos informations modiffiées sur le projet. PULL pour qu'on récupère les modifications réalisées par nos teammates ou autre contributeur du projet. La question, où sont hébergés ses projets opensource ? dans notre cas, notre REMOTE (origin) est GITHUB. Celui ci nous permet de créer des repository, de participer à des projets opensources, des projets professionnels et des projets de particulier. Il rassemble plus de 14 millions de repository.

donc notre remote principal ici dans notre état d'avancement, c'est GitHub. 
Nous pourrons dans un avenir avoir des remotes sur mon téléphone ou bien mon deuxième ordinateur.

Interéssant et à noter sur Git et GitHub, nous pouvons directemet modifier le projet sur la plateforme en ligne, ou bien en locale. il est juste important de systématiquement faire des 'git status','git commit -m/ -am', des 'git push origin master' et des 'git pull origin master'.

Si nous voulons travailler sur un repository qui en public, nous allons tout d'abord le CLONER de la manière suivante: 1° trouvons le repo qui nous intéresse, copier son URL dans la petite fenêtre à droite du projet sur GitHub. 2° Allons sur notre terminal avec Git et insérons la commande suivante : 'git clone url', cette action va ajoute l'intégralité des fichiers sur ce repository. ensuite, nous réaliserons des git push et  des git pull pour avoir les dernières modification réalisées par d'autres participants.

