# README

This repository is a test of a Rails CI/CD pipeline using a database driven app.

- Docker is used to deploy a local development app and database server
- Travis CI is set up to test the staging and master branches
- If CI passes the staging branch is deployed to a staging instance on Heroku
- On successful merge of a pull request into the master branch it is deployed into production  on Heroku

Instructions
---

To deploy docker containers locally:

docker-compose up

Site should then be accessible on localhost:3000

Push any updates to the staging branch to automatically perform CI/CD as above. Raise a pull request and merge to deploy to production.
