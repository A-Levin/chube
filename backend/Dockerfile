# backend/Dockerfile

FROM python:3.11.4

RUN mkdir /backend
WORKDIR /backend

# Install system dependencies
RUN apt-get update && \
    apt-get install -y curl && \
    apt-get clean && \
    rm -rf /var/lib/apt/lists/*

# Install Poetry
RUN curl -sSL https://install.python-poetry.org | python3 - && \
    mv /root/.local/bin/poetry /usr/local/bin/

# Copy only the dependency files to leverage Docker cache
COPY pyproject.toml ./

# Install project dependencies
RUN poetry install

# Copy the rest of the application code
COPY . .
