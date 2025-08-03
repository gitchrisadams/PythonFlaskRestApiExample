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
