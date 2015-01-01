docker-calendall
================

Calendall main application container

You can build different environment containers, for example dev:

    $ docker build -t slok/calendall:dev ./dev

You could run to test it like this:

    $ docker run --rm -it -v /home/slok/projects/calendall/calendall:/code -p 8000:8000 slok/calendall:dev ./calendall/manage.py runserver 0.0.0.0:8000


