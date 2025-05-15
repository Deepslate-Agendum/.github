# How to Use Agendum

## Requirements to Run
- python
  - modules: flask, flask_cors, typing, bson, mongoengine, functools
- docker
- reactjs
- nginx

## Running the App the First Time
1. Pull down repositories onto local machine
  - Repositories to pull down: frontend-web, backend-flask, db-mongo
2. Start docker
3. Open up a terminal that can run bash scripts in the db-mongo repository folder
  - If you are on a windows machine run `dos2unix db_initialization.sh` before opening anything
4. Run `bash startdb.sh` in the bash terminal
  - Now the `agendum-database` container should be running in docker
5. Open up a terminal in the backend-flask repository folder
6. Run `python app.py` in the terminal
7. Open up a terminal in the frontend-web repository folder
8. Run `npm run dev` in the terminal
9. In the terminal it should give you a link to click to go to `http://localhost:5173/`
10. Go to `http://localhost:5173/` and have fun!

## Running the App After the First Time
1. Start docker
2. Open up a terminal that can run bash scripts in the db-mongo repository folder
3. Run `bash startdb.sh` in the bash terminal
  - Now the `agendum-database` container should be running in docker
4. Open up a terminal in the backend-flask repository folder
5. Run `python app.py` in the terminal
6. Open up a terminal in the frontend-web repository folder
7. Run `npm run dev` in the terminal
8. In the terminal it should give you a link to click to go to `http://localhost:5173/`
9. Go to `http://localhost:5173/` and have fun!

## Closing Down the App
1. Hit Ctrl+C in the terminal that you started the frontend-web code and close it down.
2. Hit Ctrl+C in the terminal that you started the backend-flask code and close it down.
3. Run `bash stopdb.sh` in any terminal that can run bash to close down the database.

## Clearing the Database
If for any reason you wish to clear all the data you have in the app go through these steps:
1. Make sure the app is not open.
2. In a terminal that can run bash run `bash cleardb.sh`.
3. Now when you reopen the app it will not have any information.
