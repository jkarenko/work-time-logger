# Work Time Logger

## Description
This is the backend for logging work time. It is a RESTful API that allows users to log work time and retrieve work time logs.

## Technologies
- Python 3.12
- FastAPI
- SQLAlchemy
- SQLite
- Docker
- Docker Compose

## Installation
1. Clone the repository
2. Install Docker
3. Run `docker-compose up --build`
4. The API will be available at `http://localhost:8000`
5. The documentation will be available at `http://localhost:8000/docs`

## Usage
The API has two endpoints:
- `POST /work-time-logs`: This endpoint allows users to log work time. The request body should be a JSON object with the following fields:
  - `start_time`: The start time of the work log in ISO 8601 format
  - `end_time`: The end time of the work log in ISO 8601 format
- `GET /work-time-logs`: This endpoint allows users to retrieve work time logs. The response will be a JSON object with a list of work time logs.

## Configuration
The API can be configured using environment variables. The following environment variables should be set in the `.env` file:
- `DATABASE_URL`: The URL of the database. Default: `sqlite:///./app.db`
- `ACCESS_TOKEN`: The access token for the API.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
```
