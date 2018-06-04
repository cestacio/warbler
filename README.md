# Warbler

A Twitter clone web application.

[Live site](http://warbler-app.herokuapp.com/)

### Installation

```sh
# make a virtual environment
mkvirtualenv warbler
# install python requirements
pip install -r requirements.txt

# set up database
dropdb warbler-db
createdb warbler-db
flask db upgrade

# The database must be freshly created before doing this command
# If you have already added data, make sure to follow the steps above
# to reset the database.
psql warbler-db < data.sql

# start the server!
flask run
```

### Features

Added the following features to user stories, from the perspective of a user:

1.  As a user, I see custom 404 page when I try to go to an invalid URL.
1.  As a user, I see my name, location, bio, and my header image on my profile page.
1.  As a user, I can edit my name, location, bio, and my header image on my profile edit page.
1.  As a user, I can view the last 100 warbles (messages) **only from the users that I am following, and myself** rather than warbles (messages) from _all_ users.
1.  As a user, I can "like" a warble (message).
1.  As a user, I can see how many warbles (messages) I "liked" on my profile page.
