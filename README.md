django-react-heroku-s3 is a boilerplate Django server and React web app configured for Heroku and S3.

### Installation

Install requirements:

```
source env bin/activate
```

```
pip install -r requirements.txt
```

Create a .env file:

```
SECRET_KEY = '<django_secret_key>'
AWS_ACCESS_KEY_ID = '<aws_access_key_id>'
AWS_SECRET_ACCESS_KEY = '<aws_secret_access_key>'
REDIS_URL = 'redis://localhost:6379'
SENDGRID_API_KEY = '<sendgrid_api_key>'
```

Run Django server locally:

```
cd parakeet && python manage.py runserver 0.0.0.0:8000
```

Install npm depencies:

```
npm install
```

Run React app locally:
```
npm run watch
```

### Deployment

Build React app for Heroku:
```
npm run build-prod
```

Deploy to Heroku:
```
git push heroku main
```
