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


Il est aussi possible d'utiliser l'image [`jvconseil/jekyll-docker`](https://hub.docker.com/r/jvconseil/jekyll-docker) avec [`docker`](https://www.docker.com/) :

    docker run --rm \
      --volume=$(pwd):/srv/jekyll \
      -p 35729:35729 -p 4000:4000 \
      --env JEKYLL_ENV=development \
      -it jvconseil/jekyll-docker \
      jekyll serve --livereload

Pour les utilisateurices de `podman`, il faut ajouter `--env JEKYLL_ROOTLESS=1`.

Il suffit ensuite d'ouvrir son navigateur à l'adresse [http://localhost:4000/](http://localhost:4000/).
