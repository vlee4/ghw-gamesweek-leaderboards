# [GHW Games Week] Making the unofficial GHW Games Week leaderboards

Creating a Python project with flask.

## Setup

Create a .env file in the home directory.

From Auth0, under your account's dashboard > Applications > {YOUR-PROJECT} > Settings include:

```
AUTH0_CLIENT_ID=XXXX
AUTH0_CLIENT_SECRET=XXXXX
AUTH0_DOMAIN=XXXX.auth0.com
APP_SECRET_KEY=XXXX
```

From MongoDB, under your account's project > Database > Connect > Drivers > (Python Driver) include:

```
MONGO_URI=mongodb+srv://<DB_USERNAME>:<DB_PASSWORD>@<HOST>/<DB_NAME>?retryWrites=true&w=majority
```

**Note**: The auto-generated Mongo_URI may not include your DB Name, so once your DB is set up, make sure to include that where {DB_Name} is listed above.

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
`flask --app app run`
OR
`python3 app.py`

### References

- Connect Python Flask app with Auth0: https://auth0.com/docs/quickstart/webapp/python/interactive
- Flask quickstart: https://flask.palletsprojects.com/en/2.3.x/quickstart/
- Flask Forms: https://flask-wtf.readthedocs.io/en/1.0.x/quickstart/
