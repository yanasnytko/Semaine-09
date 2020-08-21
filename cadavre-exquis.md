# Cadavre Exquis - Collaboration Github

Dans le cadre de votre travail vous serez confronter au travail en équipe. Il est possible de travailler en collaboration sur le même code via Github. Pour ce faire, nous allons réaliser un petit exercice pour apprendre à partager son code avec ses collègues et comment résoudre les conflits.

## Consigne

Attribuez un numéro au hasard à chaque participant. Celui qui a le numéro 1 va réaliser l'étape 1. 

### Etape 1: Initialisation

1. Créer un `repository`sur Githube nommé `Exercice-cadavre-exquis-VotrePrénom`
2. Créer un fichier `Readme.md` (cochez "Initialize with Readme.md")
3. Avec Github Desktop, télécharger une version sur votre ordinateur.
4. Dans GH Desktop, créez une nouvelle branche `dev`
5. Publiez cette branche en cliquant sur le bouton `Publish Branch`
6. En [Markdown](https://github.com/sirius-school/Semaine-03/blob/master/theorie-markdown.md), dans VScode ajoutez un titre à votre histoire
7. Invitez les autres membres du groupe en tant que `contributors` sur Github dans les `settings > Manage Access`de votre `repository`
8. Ouvrez le fichier dans VScode et placer 1,2 ou 3 phrases l'une à la suite de l'autre.

### Etape 2: Contributions

Chaque membre qui n'est pas le numéro 1 va réaliser ces étapes

1. Allez sur le `repository` où vous avez été invité.
2. Télécharger ce `repository` avec Github Desktop.
3. Dans Github Desktop, placez-vous sur la branche `dev`
4. Ouvrez le fichier `Readme.md` et placez 1, 2 ou 3 phrases.

### Etape 3: Merge!!!

Dans l'ordre des numéros attribués, chacun va réalisez les étapes suivantes:

1. Ouvre Github Desktop, ensuite vérifiez qu'il a bien pris l'ajout de vos lignes.
2. Écrivez un message de commit et appuyez sur le bouton `Commit to Dev`
3. Cliquez ensuite sur `Push Origin`
4. (Cette étape ne sera pas dispo pour le numéro 1, passez à l'étape 11 directement) Si le `Push`ne se termine pas c'est qu'il y a un conflit. Normale vous avez probablement écrit sur les même lignes dans votre fichier. Github Desktop doit afficher une fenêtre `Newer Commits on Remote`ça veut dire qu'il y a des changement que vous ne posséder pas encore.
5. Cliquez sur `Fetch`
6. Cliquez sur `Pull Origin`
7. GHD vous montre dans quel fichier il y a un conflit, cliquez sur `Open in Visual Studio Code`
8. Corriger le fichier
9. Revenez dans GHD et cliquez sur `Commit Merge`
10. Ensuite n'oubliez pas de `Push Origin`
11. Ensuite indiquez au numéro suivant d'éffectuer la procédure de cette Etape 3
12. Si vous êtes le numéro 1, rajouter des lignes à votre fichier quand le numéro 4 aura fini, ainsi vous verrez la procédure de résolution de conflit aussi.

### Etape BONUS

1. Ramenez les commits de la branche `dev`sur `master`. Jetez un coup d'oeil à l'interface de Github Desktop...
