# Correction du TP Git Hub

Répertoire local : tpgithub

Faire d’un répertoire un repo git
- soit le répertoire existe
<pre><code>% cd tpgithub
% git init</code></pre>

- soit le répertoire est à créer
<pre><code>% git init tpgithub</code></pre>

Lier un remote (repo distant) au repo local, nommé origin
<pre><code>% git remote add origin <url du remote>

- récupérer les fichiers du remote, de la branche master, grâce au nom du remote (origin)
<pre><code>% git pull origin master</code></pre>

// sur un GitHub privé, il faut renseigner le login et le mot de passe du GitHub

- vérifier que les fichiers sont bien dans le répertoire local
<pre><code>% ls</code></pre>

- créer une branche local
<pre><code>% git branch branche1</code></pre>

- vérifier que la branche existe
<pre><code>% git branch</code></pre>

- passer sur la branche branche1
<pre><code>% git checkout branche1</code></pre>

- modifier le code de index.html pour ajouter un H2

- ajouter les fichiers au commit local
<pre><code>% git add index.html </code></pre>

//commiter la branche
<pre><code>% git commit -m "ajout du H2"</code></pre>

//push vers le remote
<pre><code>% git push origin branche1</code></pre>

// Il faut renseigner le login et le mot de passe du GitHub

Si le push ne fait rien, il faut modifier le nom d’utilisateur sur votre git local pour qu’il corresponde à votre GitHub
<pre><code>% git config --global user.username <nomUtilisateurGithub></code></pre>

A la suite de quoi, vous avez sur votre GitHub, un fichier avec un H1 sur la branche master, et un fichier avec un H1 et un H2 sur la branche branche1.
