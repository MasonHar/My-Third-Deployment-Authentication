# My Third Deployment: Authentication

App
Heroku URL: https://spu-harrism13-transactions-api-b85d0adb66ca.herokuapp.com/

Running my App (Postman)
Screenshots are in `docs/screenshots/postman`.
I tested:
- POST `/api/auth/register`
- POST `/api/auth/login`
- GET `/api/auth/me`
- PATCH `/api/auth/change-password`
- POST `/api/transactions`
- GET `/api/transactions`
- GET `/api/transactions/:id`

Running my App (Browser)
Screenshots are in `docs/screenshots/browser`.
I tested:
- `https://spu-harrism13-transactions-api-b85d0adb66ca.herokuapp.com/`
- `http://localhost:3000/`
- `http://localhost:3000/demo.html`

Differences
- deploy-app-02 does not have authentication.
- deploy-app-03 adds user registration/login with JWT.
- deploy-app-03 adds `User` model and password hashing.
- deploy-app-03 protects routes with auth middleware.
- deploy-app-03 connects transactions to users with `createdBy`.

Models
I prefer deploy-app-03 models/controllers because they include authentication and user-linked transactions, which is closer to a real app.

Challenges
- Docker was not running at first, so compose failed until I started Docker Desktop.
- Heroku config/setup took extra troubleshooting.

Questions
- None
