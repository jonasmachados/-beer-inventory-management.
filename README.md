# Bootcamp TQI Fullstack Developer Challenge - SpringBoot

This project is a challenge proposed by the Bootcamp TQI Fullstack Developer module using Spring Boot. It aims to showcase 
the implementation of a beer inventory management system.

The application provides a set of endpoints to manage beers and their related information. With these endpoints, you can 
create new beers, retrieve beers by name, list all beers, delete beers by ID, and increment the quantity of a beer.

The project utilizes JDK 11 and Spring Boot MVC framework for the backend implementation. The data is stored in an H2
Database Engine, which provides an in-memory database solution.

To get started with the project, you can clone the repository, import it into your preferred IDE, build and run the 
project using Maven or your IDE's tools. Once the project is up and running, you can access the application in your browser 
at `http://localhost:8080`.

Feel free to explore the provided endpoints and manage the beer inventory according to your requirements.


## Endpoints

| Endpoint                                 | Method | Description                                          | Request Body  | Response           | HTTP Status |
|------------------------------------------|--------|------------------------------------------------------|---------------|--------------------|-------------|
| `/api/v1/beers`                          | POST   | Creates a new beer.                                  | BeerDTO       | BeerDTO            | 201 (Created)|
| `/api/v1/beers/{name}`                    | GET    | Retrieves a beer by its name.                        | -             | BeerDTO            | 200 (OK)    |
| `/api/v1/beers`                          | GET    | Retrieves a list of all beers.                       | -             | List of BeerDTO    | 200 (OK)    |
| `/api/v1/beers/{id}`                      | DELETE | Deletes a beer by its ID.                            | -             | -                  | 204 (No Content)|
| `/api/v1/beers/{id}/increment`            | PATCH  | Increments the quantity of a beer.                   | QuantityDTO   | BeerDTO            | 200 (OK)    |

## Technologies Used
- JDK 11
- Spring Boot MVC
- H2 Database Engine

## Installation
1. Clone the repository: `git clone https://github.com/your-username/your-repository.git`
2. Import the project into your IDE
3. Build and run the project using Maven or your IDE's tools
4. Access the application in your browser: `http://localhost:8080`

## Database
The project uses the H2 Database Engine.

