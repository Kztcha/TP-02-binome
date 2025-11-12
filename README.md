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

# **IV. Étape 4: Création d'un dépôt sur GitHub et push**

**14 :**

* `git remote add origin [URL]` : lie le dépôt local au dépôt distant.
* `git push -u origin master` : envoie la branche *master* vers le dépôt distant et définit *origin/master* comme suivi par défaut.
* `git push --set-upstream origin master` : même fonction que la précédente, syntaxe alternative.

**15 :**

* `git clone URL` : crée un nouveau dépôt local à partir d’un dépôt distant.
* `git remote add origin URL` : ajoute un dépôt distant à un dépôt local déjà existant.

# **V. Étape 5:  Collaboration - Clonage et modifications**

**21 :**

* Création du répertoire: mkdir TP-Binome, on se place dedans: cd TP-Binome puis on clone le depot: git clone <https://github.com/Kztcha/TP-02-binome>

**22 :**

* Modifier le fichier: éditeur README.md, ajouter et commiter les changements: git add README.md puis git commit -m "Modification du README.md"

**23 :**

* Pousser les modifications: git push origin main

**24 :**

* L'etudiant 1 recupere les modifications avec git pull origin main

**25 :**    

- Apres avoir utiliser les commandes git push et git pull avec l’option origin main une fois , il n'est plus nécessaire d'utiliser l'option les fois suivantes.



# **VI. Étape 6: Gestion des conflits**



**26:**

Ligne test
$ git push
To https://github.com/Kztcha/TP-02-binome
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/Kztcha/TP-02-binome'
hint: Updates were rejected because the remote contains work that you do not
hint: have locally. This is usually caused by another repository pushing to
hint: the same ref. If you want to integrate the remote changes, use
hint: 'git pull' before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.


# **VII. Étape 7:  Comprendre la différence entre git pull et git fetch**

**29 :**

* ÉTUDIANT A crée un nouveau dépôt sur GitHub et y ajoute un fichier notes.txt avec le 
contenu "Première note". Commitez: git commit -m "EA : premier commit » 

**31 :**

*On se place dans le dossier puis clone le depot : git clone https://github.com/....

**32 :**

*git add notes.txt
*git commit -m "Deuxieme note"
*git push

**34 :**

*Apres git fetch on remarque que le deuxieme étudiant ne voit pas cette nouvelle Ligne

**35 :**

*Le git log du deuxieme étudiant ne contient pas encore le commit de la deuxième note.