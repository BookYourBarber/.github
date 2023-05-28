# Welcome to BookYourBarber!

Welcome to my BookYourBarber open-source school project, providing a user-friendly platform for booking barber appointments with ease and convenience!

# Running the project
## Clone the main repository
To run the project, you will need docker and its compose installed (see [here](https://docs.docker.com/engine/install/)).

Firstly you should clone the main repository [BookYourBarber](https://github.com/BookYourBarber/BookYourBarber) in which one are all existing repositories.

When you clone it, your file tree should look like this:

```
├── appointments
│   ├── app.js
│   ├── Dockerfile
│   ├── index.js
│   ├── jest.config.js
│   ├── package.json
│   ├── package-lock.json
│   ├── routers
│   │   └── appointmentRouter.js
│   ├── sonar-project.properties
│   ├── tests
│   │   └── appointmentRouter.test.js
│   └── utils.js
├── customer_frontend
│   ├── Dockerfile
│   ├── package.json
│   ├── package-lock.json
│   ├── public
│   │   ├── favicon.ico
│   │   ├── imgs
│   │   │   ├── asdf.png
│   │   │   ├── bluemappin.png
│   │   │   ├── home.png
│   │   │   ├── rainbow_adobe_express.svg
│   │   │   └── rainbow.png
│   │   ├── index.html
│   │   ├── logo192.png
│   │   ├── logo512.png
│   │   ├── manifest.json
│   │   └── robots.txt
│   ├── README.md
│   └── src
│       ├── App.css
│       ├── App.js
│       ├── App.test.js
│       ├── Components
│       │   ├── Appointment.jsx
│       │   ├── Footer.js
│       │   ├── Header.js
│       │   ├── Maps.jsx
│       │   ├── Schedule.jsx
│       │   └── UserInformation.jsx
│       ├── index.css
│       ├── index.js
│       ├── logo.svg
│       ├── Pages
│       │   ├── AppointmentPage.js
│       │   ├── HomePage.js
│       │   └── UserInformation.js
│       ├── reportWebVitals.js
│       └── setupTests.js
├── docker-compose.yml
├── package.json
├── package-lock.json
├── README.md
├── schedule
│   ├── app.js
│   ├── Dockerfile
│   ├── index.js
│   ├── jest.config.js
│   ├── package.json
│   ├── package-lock.json
│   ├── routers
│   │   └── scheduleRouter.js
│   └── tests
│       └── scheduleRouter.test.js
├── time_slots
│   ├── Dockerfile
│   ├── index.js
│   ├── package.json
│   ├── package-lock.json
│   └── routers
│       └── timeSlotRouter.js
└── users
    ├── app.js
    ├── Dockerfile
    ├── index.js
    ├── jest.config.js
    ├── package.json
    ├── package-lock.json
    ├── routers
    │   └── userRouter.js
    └── tests
        └── userRouter.test.js


```
Before you start the application you should there is two things you should set.

1. You should go to every folder you should run ```npm install``` so you install required dependencies
2. You have to add ```.env``` file in ```frontend_customer``` and set ***google maps API key*** so application can work. Follow the instructions [here](https://github.com/BookYourBarber/bub_customer_frontend) 



Go to root folder and run docker compose up --build in your terminal.
The frontend application is now available on deafult port http://localhost:3000
