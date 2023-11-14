# emu
A curiosity project

docker-compose -f docker-compose.prod.yml up -d --build

once the git project is cloned, create environment files for running locally

$.env.dev
FLASK_APP=project/__init__.py
FLASK_DEBUG=1
DATABASE_URL=postgresql://hello_flask:hello_flask@db:5432/hello_flask_dev
SQL_HOST=db
SQL_PORT=5432
DATABASE=postgres
APP_FOLDER=/usr/src/app


$.env.prod
FLASK_APP=project/__init__.py
FLASK_DEBUG=0
DATABASE_URL=postgresql://hello_flask:hello_flask@db:5432/hello_flask_prod
SQL_HOST=db
SQL_PORT=5432
DATABASE=postgres
APP_FOLDER=/home/app/web


$.env.prod.db
POSTGRES_USER=hello_flask
POSTGRES_PASSWORD=hello_flask
POSTGRES_DB=hello_flask_prod