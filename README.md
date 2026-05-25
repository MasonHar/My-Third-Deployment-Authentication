# My Third Deployment: Authentication

App
Heroku URL: https://spu-harrism13-transactions-api-b85d0adb66ca.herokuapp.com/

Running my App (Postman)
Screenshot 1 - Register user
![Screenshot 1 - Register user](Screenshot%202026-05-24%20233651.png)

Screenshot 2 - Create transaction
![Screenshot 2 - Create transaction](Screenshot%202026-05-24%20234619.png)

Screenshot 3 - Get transactions
![Screenshot 3 - Get transactions](Screenshot%202026-05-24%20234709.png)

Screenshot 4 - Get transaction by id
![Screenshot 4 - Get transaction by id](Screenshot%202026-05-24%20235130.png)

Screenshot 5 - Get me with token
![Screenshot 5 - Get me with token](Screenshot%202026-05-25%20000836.png)

Screenshot 6 - Get me without token
![Screenshot 6 - Get me without token](Screenshot%202026-05-25%20000854.png)

Running my App (Browser)
Screenshot 1 - Browser app URL
![Screenshot 1 - Browser app URL](Screenshot%202026-05-24%20233554.png)

Screenshot 2 - Localhost root
![Screenshot 2 - Localhost root](Screenshot%202026-05-25%20000144.png)

Screenshot 3 - Localhost demo page
![Screenshot 3 - Localhost demo page](Screenshot%202026-05-25%20000225.png)

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
