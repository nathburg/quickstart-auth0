# Quickstart Instructions

Add a .env file to your project. Give it these variables:

```
AUTH0_CLIENT_ID=
AUTH0_CLIENT_SECRET=
AUTH0_DOMAIN=
```

You can find the values to give these variables in the Settings of your Auth0 app. They're in Basic Information.

In the Settings of your Auth0 app, under Application URIs

-   add `http://127.0.0.1:3000/callback/` in Allowed Callback URLs
-   add `http://127.0.0.1:3000/` in Allowed Logout URLs

Now in the terminal run

```
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver 3000
```

The app should now be running at http://localhost:3000.
