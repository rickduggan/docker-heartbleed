docker-heartbleed
=================

Dockerfile to install and run heartbleed (https://github.com/FiloSottile/Heartbleed).

Usage:

  1) Install docker (https://www.docker.io/gettingstarted/#h_installation)

  2) Build heartbleed image once:

     docker build -t <yourname>/heartbleed https://raw.githubusercontent.com/kasimon/docker-heartbleed/master/Dockerfile

  3) Run Heartbleed from image:

     $ docker run <yourname>/heartbleed github.com:443
     2014/04/09 10:37:28 github.com:443 - SAFE

  4) (optional) Create alias:

    $ alias heartbleed="docker run <yourname>/heartbleed"
    $ heartbleed github.com:443
    2014/04/09 10:37:28 github.com:443 - SAFE

