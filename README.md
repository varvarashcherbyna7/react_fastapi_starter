# Node 10+
# python 3.6

node --version
v14.15.0

python3 --version
Python 3.8.4

pip3 --version
pip 20.1.1

npm --version
6.14.8


Frontend

cd frontend
# Install dependencies
npm install
# npm run start which starts the server
npm run start
# open localhost: 3000

Backend

cd backend
python3 -m venv .venv
source env/bin/activate
pip install -r requirements.txt
pip list
cd src
uvicorn api:app --reload




# Adding new software dependencies - such as newsapi-python
# make sure virtual env is activated
source env/bin/activate
pip install newsapi-python
# Freeze your current dependencies to the requirements.txt file.
pip freeze > requirements.txt
# Go to directory backend/src where the api.py is.
cd backend/src
# Run the app using uvicorn server in reload mode. Changing files in src, will cause the server to automatically load your changes.
uvicorn api:app —-reload
