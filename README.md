# A small University API using FastAPI.

## The API supports these endpoints:

- GET / returns a welcome page with API information.
- GET /students returns all students.
- GET /students/{student_id} returns one student by ID.
- If the student does not exist, return a 404 JSON error.


## Install requirements

First generate a venv:

``` python3 -m venv .venv ```

```source .venv/bin/activate```

Than install the requirements:

```python -m pip install -r requirements.txt```

## How to run

```uvicorn main:app --reload```

## Test

URLs to test:

```http://127.0.0.1:8000/```

```http://127.0.0.1:8000/students/```

```http://127.0.0.1:8000/students/s1```

```http://127.0.0.1:8000/students/s10```
