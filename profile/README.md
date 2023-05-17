# Welcome to BookYourBarber!

Welcome to my BookYourBarber open-source school project, providing a user-friendly platform for booking barber appointments with ease and convenience!

# Running the project
## Clone the main repository
Firstly you should clone the main repository ([BookYourBarber](https://github.com/BookYourBarber/BookYourBarber)) in which one are all the existing repositories.

To run the project, you will need docker and its compose installed (see here). The compose file is as follows:
```
version: '3'
services:
  client_information:
    container_name: customer_frontend_home
    build: ./customer_frontend
    volumes:
      - ./customer_frontend:/usr/src/app
    ports:
      - "3000:3000"
    restart: always
    # environment:
    #   CONN_URL: ""

  users:
    container_name: users_api
    build: ./users
    volumes:
      - ./users:/usr/src/app
    ports:
      - "5001:5001"
    restart: always

  schedule:
    container_name: schedule_api
    build: ./schedule
    volumes:
      - ./schedule:/usr/src/app
    ports:
      - "5002:5002"
    restart: always

  appointments:
    container_name: appointments_api
    build: ./appointments
    volumes:
      - ./appointments:/usr/src/app
    ports:
      - "5003:5003"
    restart: always

  timeslots:
    container_name: time_slots_api
    build: ./time_slots
    volumes:
      - ./time_slots:/usr/src/app
    ports:
      - "5004:5004"
    restart: always
```
