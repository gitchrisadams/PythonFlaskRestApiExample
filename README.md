# PythonFlaskRestApiExample

This repo is an example of a Rest api that uses GET, POST, PUT, DELETE and does CreateReadUpdateDelete(CRUD) operations.

## Create a new python env and activate

python -m venv .venv
source .venv/scrpts/Activate

## Install Flask

pip install flask

## Run the server

flask run

## Access api endpoint in browser

Example:
http://localhost:5000/stores

## API requests:

## GET - Get all stores:

http://localhost:5000/store

## Create a new store

## POST - Create a store

http://localhost:5000/store

#### Add to body:

`{
"items": [],
"name": "Store 2"
}`

## POST - Create an item

http://localhost:5000/store/Store 2/item
Where Store 2 is the name of store to create

### Add to body:

`{
	"name": "lamp",
	"price": 2
}`

## GET - Get a specific store

http://localhost:5000/store/MyStore

## GET - Get specific store items

http://localhost:5000/store/MyStore/item

# Docker

## Building the docker image from the Dockerfile

`docker build -t rest-apis-flask-python-udemy .`

Where rest-apis-flask-python-udemy is the name you want to tag the images with

# Edit the port on the created docker file

## Docker Desktop

If using Docker Desktop, be sure to forward port 5005 to 5000
When you click on "run" in Docker desktop then go to optional
settings, you will see Ports > Local Host
Be sure to put 5005 in "Local Host"
Then click "Run"

## Command line

Instead of using Docker Desktop you can use the command line
`docker run -p 5005:5000 rest-apis-flask-python`

## Docker Compose

## Starting docker compose

`docker compose up`

# Rquirements .txt file (requirements.txt)

Run this to install:
`pip install -r requirements.txt`
