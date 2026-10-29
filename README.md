# RESTful-API

Practice projects for building REST APIs with Django and Django REST Framework. Each folder is a separate Django project.

## Projects

| Folder | Description |
|---|---|
| `backend/` | Todo API (`Todo`: title, body) with list and detail endpoints |
| `blogapi/` | Blog API: posts and users, owner-only permissions, token auth (`dj-rest-auth`, `allauth`), CORS, Swagger and ReDoc docs |
| `library/` | Library API (`books` + `api` apps), early stage |
| `frontend/` | Create React App skeleton (default template, not connected yet) |

## Technologies

Python, Django, Django REST Framework, dj-rest-auth, django-allauth, django-cors-headers, drf-yasg (Swagger/ReDoc), SQLite, React (frontend skeleton).

## How to Run

There is no `requirements.txt` yet; install the packages manually.

```bash
git clone https://github.com/MShabani-dev/RESTful-API.git
cd RESTful-API/blogapi          # or backend / library
python -m venv .venv && source .venv/bin/activate
pip install django djangorestframework dj-rest-auth django-allauth django-cors-headers drf-yasg
python manage.py migrate
python manage.py runserver
```

Blog API endpoints (`blogapi`):
- `/api/v1/` posts, `/api/v1/users/` users
- `/api/v1/rest-auth/` login/logout, `/api/v1/rest-auth/registration/` sign up
- `/swagger/` and `/redoc/` interactive docs


## Status

Learning repository; `library/` and `frontend/` are incomplete.
