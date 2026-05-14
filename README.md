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
<img width="1919" height="966" alt="image" src="https://github.com/user-attachments/assets/b7ffdd24-877e-4044-bed8-1ddcd84fbff5" />
<img width="1671" height="480" alt="image" src="https://github.com/user-attachments/assets/021207e3-db0f-447d-8f8f-b169933c370c" />
<img width="1722" height="906" alt="image" src="https://github.com/user-attachments/assets/9aeb426e-3e79-4d9a-a8f6-7f0239988e3f" />


