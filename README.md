# Correction du TP Git Hub

Répertoire local : tpgithub

Faire d’un répertoire un repo git
- soit le répertoire existe

    % cd tpgithub
    % git init

- soit le répertoire est à créer

  % git init tpgithub


-lier un remote (repo distant) au repo local, nommé origin
% git remote add origin <url du remote>

- récupérer les fichiers du remote, de la branche master, grâce au nom du remote (origin)
% git pull origin master

// sur un GitHub privé, il faut renseigner le login et le mot de passe du GitHub

- vérifier que les fichiers sont bien dans le répertoire local
% ls

- créer une branche local
% git branch branche1

- vérifier que la branche existe
% git branch

- passer sur la branche branche1
% git checkout branche1

- modifier le code de index.html pour ajouter un H2

- ajouter les fichiers au commit local
% git add index.html 

//commiter la branche
% git commit -m "ajout du H2"

//push vers le remote
% git push origin branche1

// Il faut renseigner le login et le mot de passe du GitHub

Si le push ne fait rien, il faut modifier le nom d’utilisateur sur votre git local pour qu’il corresponde à votre GitHub
% git config --global user.username <nomUtilisateurGithub>

A la suite de quoi, vous avez sur votre GitHub, un fichier avec un H1 sur la branche master, et un fichier avec un H1 et un H2 sur la branche branche1.
