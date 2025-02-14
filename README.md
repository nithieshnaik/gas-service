# Gas Service Backend

## Overview
This is the backend for the Gas Service application, built using **Django** for API management and **React** for the frontend. It includes user authentication, service request handling, and payment processing.

## Technologies Used
- **Backend:** Django, Django REST Framework
- **Database:** PostgreSQL
- **Frontend:** React
- **Authentication:** JWT
- **Task Queue:** Celery with Redis

## Setup Instructions
### Prerequisites
- Python 3.10+
- PostgreSQL
- Node.js & npm (for frontend, if applicable)

### Installation Steps
1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-repo/gas-service-backend.git
   cd gas-service-backend
   ```
2. **Create and activate a virtual environment:**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```
3. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```
4. **Configure environment variables:**
   - Create a `.env` file and add your database and secret settings.
5. **Run migrations:**
   ```bash
   python manage.py migrate
   ```
6. **Create a superuser (admin):**
   ```bash
   python manage.py createsuperuser
   ```
7. **Run the development server:**
   ```bash
   python manage.py runserver
   ```

## API Documentation
The API endpoints are documented using **Swagger/OpenAPI**. Once the server is running, visit:
- `http://localhost:8000/api/docs/`


## Deployment
1. Set up a production database (PostgreSQL).
2. Configure a WSGI server (Gunicorn) and reverse proxy (NGINX).
3. Use Docker for containerized deployment if needed.

## Contact & Contributions
For contributions, submit a pull request or open an issue.

Maintained by: Nithiesh Naik


