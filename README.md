# **I. 1. Étape 1: Configuration initiale**

    1: git config --global user.name "NOM"

    2: git config --global user.email "EMAIL"

    3: git config --list

# **II.Étape 2: Création d'un dépôt local**

    4: On utilise `git init` quand on veut **initialiser un dépôt Git dans un dossier déjà existant**.

`git init NomDuDépôt` sert à **créer un nouveau dossier "NomDuDépôt" et à y initialiser un dépôt.

    5: git init

    6: si on est pas positionner dans le depot il faut faire : cd "nomdudepot"

    7:  git branch pour verifier les branches existantes, si master n'existe pas il faut faire : git checkout master

    8 & 9 : $ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")
