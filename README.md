# Home Rental Service

This repo contains a Django project in the `Flat_Rent_django` folder.

## Deployment

The Django app is configured for deployment with:

- `Flat_Rent_django/requirements.txt`
- `Flat_Rent_django/Procfile`
- `Flat_Rent_django/runtime.txt`

### Recommended deployment flow

1. Push this repository to GitHub (already done).
2. Use a host like Render, Railway, Fly.io, or Heroku.
3. Set the deployment root to `Flat_Rent_django`.
4. Use the following build steps:
   - `pip install -r requirements.txt`
   - `python manage.py migrate`
   - `python manage.py collectstatic --noinput`
5. Use the start command from `Procfile`.

### Environment variables

- `DJANGO_SECRET_KEY` - your production secret
- `DJANGO_DEBUG` - `False` in production
- `DJANGO_ALLOWED_HOSTS` - comma-separated hostnames
- `DATABASE_URL` - PostgreSQL URL for production

## Local development

From `Flat_Rent_django`:

```bash
python manage.py runserver
```
