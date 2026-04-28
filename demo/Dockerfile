FROM python:3.11-slim

WORKDIR /demo

RUN apt-get update && apt-get install -y gcc libpq-dev && rm -rf /var/lib/apt/lists/*

RUN pip install poetry

COPY pyproject.toml poetry.lock ./

RUN poetry config virtualenvs.create false \
    && poetry install --no-interaction --no-ansi --no-root --without dev

COPY . .

CMD ["uvicorn", "demo.src.demo:app", "--host", "0.0.0.0", "--port", "8000"]
