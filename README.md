# Dealership Review App

This project is a full-stack application for managing dealership reviews. It includes a backend server built with Node.js and Express, a frontend built with React, and a MongoDB database.

## Project Structure

```
.github/
  workflows/
    main.yml
.gitignore
LICENSE
README.md
server/
  database/
    app.js
    data/
      dealership.js
    docker-compose.yml
    Dockerfile
    inventory.js
    package.json
    review.js
  deployment.yaml
  djangoapp/
    __init__.py
    .env
    admin.py
    apps.py
    microservices/
    models.py
    populate.py
    restapis.py
    urls.py
    views.py
  djangoproj/
    __init__.py
    asgi.py
    settings.py
    urls.py
    wsgi.py
  Dockerfile
  entrypoint.sh
  frontend/
    ...
  manage.py
  package.json
  requirements.txt
```

## Backend

The backend server is located in the `server/database` directory. It uses Express for handling HTTP requests and Mongoose for interacting with MongoDB.

### Setup

1. Navigate to the `server/database` directory:
   ```sh
   cd server/database
   ```

2. Install the dependencies:
   ```sh
   npm install
   ```

3. Start the server:
   ```sh
   npm start
   ```

The server will run on `http://localhost:3030`.

### API Endpoints

- `GET /`: Welcome message
- `GET /fetchDealers/:state`: Fetch dealers by state
- `GET /fetchDealer/:id`: Fetch dealer by ID
- `POST /insert_review`: Insert a new review

## Frontend

The frontend is located in the frontend directory. It is built with React and uses React Router for navigation.

### Setup

1. Navigate to the frontend directory:
   ```sh
   cd server/frontend
   ```

2. Install the dependencies:
   ```sh
   npm install
   ```

3. Start the development server:
   ```sh
   npm start
   ```

The app will run on `http://localhost:3000`.

### Available Scripts

In the project directory, you can run:

- `npm start`: Runs the app in development mode.
- `npm test`: Launches the test runner.
- `npm run build`: Builds the app for production.
- `npm run eject`: Ejects the app from Create React App.

## License

This project is licensed under the Apache License 2.0. See the LICENSE file for details.
