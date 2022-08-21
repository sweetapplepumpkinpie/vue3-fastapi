## Backend API
The backend is a REST API built in Python and using FastAPI.

Uses: 
- Pydantic (validation between frontend input & backend output, conversion from DB ORM models)
- SQLAlchemy (DB abstraction, ORM models)
- python-jose is used for working with JWT
- passlib & argon2 is used for handling password hashing
- Poetry is used for dependency management

The API exposes two endpoints:
- `GET /` returns a JSON Hello World result, protected by OAuth2
- `POST /token` takes multi-part form data providing credentials for logging in & returns an OAuth2 bearer token

## Frontend UI
The frontend is a Vue3.js app that presents a very basic Login form with Username & Password fields.

Uses:
- Vue3.js for app framework 
- Element-Plus as UI framework
- VueX for state management
- Vue-router for handling routing
- Native Fetch API for communication with the backend REST API

# Contributing
Please feel free to submit PRs if you feel you can improve the demo.
