# [GHW Games Week] Making the unofficial GHW Games Week leaderboards

Creating a Python project with flask.

## Setup

Create a .env file in the home directory.

From Auth0 include:

```
AUTH0_CLIENT_ID=XXXX
AUTH0_CLIENT_SECRET=XXXXX
AUTH0_DOMAIN=XXXX.auth0.com
APP_SECRET_KEY=XXXX
```

From MongoDB include:

```
MONGO_URI=mongodb+srv://<DB_USERNAME>:<DB_PASSWORD>@<HOST>/<DB_NAME>?retryWrites=true&w=majority
```

## Create a Python virtual environment

On Mac/Linux:
`python3 -m venv .venv`

On Windows:
`py -3 -m venv .venv`

## Activate Python virtual environment

For Mac/Linux:
`. .venv/bin/activate`

For Windows:
`.venv\Scripts\activate`

## Run project

In the terminal run:
`flask --app hello run`

### References

Flask quickstart: `https://flask.palletsprojects.com/en/2.3.x/quickstart/`
