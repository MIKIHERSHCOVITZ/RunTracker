# RunTracker
RunTracker is a jogging route tracking application that allows users to filter and view jogging routes in their area.

The application shows the routes on a map and provides detailed information about each route.

Users can also add information to routes and, in the future, will be able to record and add new routes.

## Features

Filter Routes by Radius: Users can filter jogging routes within a specified radius.

View Route Details: Users can click on a starting point of a route to see detailed information about it.

Add Information to Routes: Users can add information to a route after completing their jog.

Record New Routes (Coming Soon): Users will be able to record new jogging routes and add information about them.

## Technologies Used

Frontend: React Native

Backend: Python

Serverless Framework: Azure Functions

Geolocation: Uses device location services to track routes

## Project Structure
```
RunTracker/
├── frontend/
│   ├── App.js
│   ├── app.json
│   ├── babel.config.js
│   ├── package.json
│   │
│   ├── assets/
│   │   ├── ... # Not important
│   │
│   ├── screens/
│   │   ├── HomeScreen.js
│   │   ├── RouteDetailsScreen.js
│   │   ├── UpdateRouteScreen.js
│   │   └── LoginScreen.js
│
└── backend/
    ├── requirements.txt
    ├── host.json
    ├── CollectCoordination/
    │   ├── __init__.py
    │   └── function.json
    ├── GetRoutes/
    │   ├── __init__.py
    │   └── function.json
    ├── RemoveRoute/
    │   ├── __init__.py
    │   └── function.json
    ├── SignIn/
    │   ├── __init__.py
    │   └── function.json
    ├── SignUp/
    │   ├── __init__.py
    │   └── function.json
    └── UpdateRoute/
        ├── __init__.py
        └── function.json
```

## Installation

Note: The app runs on Azure, if you want to run it locally, please change the api's to match the local settings.

Replace 'https://assignment1-sophie-miki-omer.azurewebsites.net' with 'http://localhost:7071'.

1. **Clone the repository:**

```bash
git clone https://github.com/MIKIHERSHCOVITZ/RunTracker.git
cd RunTracker
```

2. **Set up a virtual environment:**

```bash
python -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`
```

3. **Running the Frontend:**

```bash
cd frontend
npm install
npm start
```

4. **Running the Backend:**

```bash
cd backend
pip install -r requirements.txt
func start
```