Digits Recognizer
=================

Fullstack handwritten digits recognizer project with TensorFlow, OpenCV, Django, and React.

![ScreenFlow](https://user-images.githubusercontent.com/9797761/134186945-8f1d12c3-ef05-4bb7-9ee2-5730511d2763.gif)

Run the app on local machine
----------------------------

Ensure that you have Python 3.8+, Pipenv, and recent Node.js installed on your local machine.

**To run the backend server:**

1.  Change to the `backend/` directory and install the dependencies:

        cd backend
        pipenv install 

2.  Run the development server:

        ppienv run python manage.py runserver

    It will run Django's development server on port 8000.
        
3.  Open `http://localhost:8000` with your browser to see the welcome message.

**To run the frontend app:**

1.  Change to the `frontend/` directory and install the dependencies:

        cd frontend
        yarn install

2.  Run the server:

        yarn start

3.  Open `http://localhost:3000` with your browser to see the frontend app.

Run the app on local machine with Docker
----------------------------------------

Ensure that you have Docker and Docker Compose installed on your machine. Run:

    docker-compose up

to build and run the containers, then open `http://localhost:3000` with your browser 
to see the frontend app.

If you want to run on machine other than localhost (e.g: EC2 instance), you need to 
pass `FRONTEND_URL` and `BACKEND_URL` variables so both frontend and backend understand 
how to talk to each other:

    FRONTEND_URL=http://1.2.3.4:3000 BACKEND_URL=http://1.2.3.4:8000 docker-compose up
