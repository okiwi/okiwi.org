Dépot de code central du site d'Okiwi
=====================================

Dépendances
-----------

 *  ruby 2.0
 *  jekyll 1.4.3 ou supérieur


Installation
------------

[Jekyll](http://jekyllrb.com/docs/home/)  est un générateur de sites statiques. Pour l'installer il faut avoir ruby et la commande gem d'installée.


    gem install jekyll



Lancer un serveur local
-----------------------

    git clone git@github.com:okiwi/okiwi.org.git
    cd okiwi.org
    jekyll serve


Il est aussi possible d'utiliser l'image [`jekyll/builder`](https://github.com/envygeeks/jekyll-docker#readme) avec [`docker`](https://www.docker.com/) :

    docker run --rm \
      --volume=$(pwd):/srv/jekyll \
      --net=host \
      -p 35729:35729 -p 4000:4000 \
      --env JEKYLL_ENV=development \
      -it jekyll/builder \
      jekyll serve --livereload


Il suffit ensuite d'ouvrir son navigateur à l'adresse [http://localhost:4000/](http://localhost:4000/).
