# FastAPI Task Manager

*A production-ready Task Management API built with FastAPI, PostgreSQL, and async SQLAlchemy.*

---

## Features

- *Task CRUD*: Create, read, update, soft-delete tasks.
- *Comments*: Add and retrieve comments for tasks.
- *Filtering & Pagination*: Filter by status, priority, assignee; paginate results.
- *Analytics*: Real-time task analytics (counts, averages, top assignees).
- *Role-based Access*: JWT-based authentication for secure task operations.
- *Async & Scalable*: Fully asynchronous with PostgreSQL and Redis caching.
- *Background Tasks*: Audit logs for task updates.
- *Testing*: Unit and integration tests with pytest & pytest-asyncio.

---

## Tech Stack

- *Backend*: FastAPI  
- *Database*: PostgreSQL (async with SQLAlchemy)  
- *Caching*: Redis  
- *Testing*: pytest, pytest-asyncio  
- *Containerization*: Docker & docker-compose  

---

## Getting Started

### 1. Clone Repository

```bash
git clone https://github.com/<Sowbhagya430>/fastapi-task-manager.git
cd fastapi-task-manager

2. Create .env file

Use the following variables:

POSTGRES_USER=postgres
POSTGRES_PASSWORD=Krishna1437
POSTGRES_DB=task_manager
POSTGRES_HOST=localhost
POSTGRES_PORT=5432

3. Create & Activate Virtual Environment

python -m venv venv
source venv/bin/activate   # Linux/Mac
venv\Scripts\activate      # Windows

4. Install Dependencies

pip install -r requirements.txt

5. Run Migrations / Create Tables

# Tables are auto-created on startup using SQLAlchemy

6. Run the API

uvicorn main:app --reload

Visit http://127.0.0.1:8000/docs for Swagger UI.


---

Docker Setup

docker-compose up --build

This will start the FastAPI app, PostgreSQL, and Redis.


---

Testing

Run all tests:

pytest --asyncio-mode=auto


---

Project Structure

fastapi-task-manager/
│
├─ main.py
├─ database.py
├─ models.py
├─ schemas.py
├─ tasks.py
├─ test_main.py
├─ requirements.txt
├─ Dockerfile
├─ docker-compose.yml
└─ .env


---

License

MIT License
