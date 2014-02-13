Dépot de code central du site d'Okiwi
=====================================

Dépendances
-----------

 *  ruby 2.0
 *  jekyll 1.4.3 ou supérieur
 *  yuicompressor pour minifier CSS


Installation
------------

[Jekyll](http://jekyllrb.com/docs/home/)  est un générateur de sites statiques. Pour l'installer il faut avoir ruby et la commande gem d'installée.


    gem install jekyll



Lancer un serveur local
-----------------------

    git clone git@github.com:okiwi/okiwi.org.git
    cd okiwi.org
    jekyll server --watch


Il suffit ensuite d'ouvrir son navigateur à l'adresse [http://localhost:4000/](http://localhost:4000/) 


Minifier CSS
------------

Pour minifier le CSS j'utilise yuicompressor sur Webstorm avec la commande suivante :

    /usr/local/bin/yuicompressor $FileName$ -o $FileNameWithoutExtension$.min.css

