# django-postgres Test Project

This test project contains Python tests of the various pieces of API
functionality implemented by django-postgres. More tests exist in `../tests/`.

To run the tests:

1.  Install Postgres. I use [Postgres.app](http://postgresapp.com/).

2.  Create a `django_postgres` database:

       $ psql
       psql (9.1.4)
       Type "help" for help.

       johndoe=# CREATE DATABASE django_postgres;
       CREATE DATABASE

3.  Run `make test` from this directory. This will create a virtualenv, install
    the test project requirements, and execute the tests. On subsequent runs,
    the virtualenv/installation steps will be skipped thanks to the Makefile.
