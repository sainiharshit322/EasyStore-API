# API Key Generator

A project for generating and managing API keys securely.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Configuration](#configuration)
- [Contributing](#contributing)
- [License](#license)

## Introduction

This project provides a secure and efficient way to generate and manage API keys for your applications. It includes a web interface for generating new keys, viewing existing keys, and revoking keys as needed.

## Features

- Secure API key generation
- Web interface for managing keys
- Integration with Redis for caching and performance
- Database support for persistent storage

## Installation

### Prerequisites

Ensure you have the following software installed:

- Python 3.x
- pip
- Redis

### Steps

1. Clone the repository:
    ```bash
    git clone hhttps://github.com/iam-tsr/API-Key-Generator.git
    cd API-Key-Generator
    ```

2. Set up a virtual environment:
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. Install the dependencies:
    ```bash
    pip install -r requirement.txt
    ```
    ```bash
    pip install redis google-auth google-auth-oauthlib google-auth-httplib2 google-api-python-client
    ```

## Usage

### Running the Application

To run the application locally:

```bash
streamlit run /workspaces/API-Key-Generator/app.py
```

### Accessing the Application

Once the application is running, you can access it at `http://127.0.0.1:5000`.

## Configuration

### Redis Configuration

Ensure Redis is installed and running on your machine. You can configure Redis settings in the `redis.conf` file.

## Project Structure

Here's an overview of the project's structure:

```
.
├── .env
├── .venv
├── alembic.ini
├── alembic/
├── api.py
├── api_keys.db
├── app.py
├── credentials.json
├── data/
├── dump.rdb
├── redis.conf
├── redis.log
├── redis_config.py
├── requirement.txt
├── static/
├── templates/
├── test.db
├── token.pickle
├── upload_to_drive.py
└── venv/
```

- **app.py**: Main application file.
- **api.py**: API routes for key management.
- **alembic/**: Database migration scripts.
- **templates/**: HTML templates for the web interface.
- **static/**: Static files (CSS, JS).
- **redis_config.py**: Configuration for Redis.
- **requirement.txt**: List of dependencies.
- **credentials.json** and **token.pickle**: Credentials for accessing external services (if applicable).

## Feedback and Contributions:

Feedback and contributions to improve this program are welcome. Feel free to open an issue or submit a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE.txt) file for details.