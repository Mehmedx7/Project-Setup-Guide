# Project-Setup-Guide

[OCPP Backend] is a Django project that utilizes ASGI with Redis/Memurai as a channel layer.

## Prerequisites

Before you begin, ensure you have the following installed on your system:

- Python (version latest stable)
- Redis or Memurai
- Your preferred IDE (e.g., VSCode, PyCharm)

## Django Setup

1. **Clone the Repository:**

    ```bash
    git clone <Your URL>
    ```

2. **Go to Your Project Folder:**

    ```bash
    cd fmt-backend
    ```


3. **Install Dependencies:**

    ```bash
    pip install -r requirements.txt
    ```

4. **Apply Migrations:**

    ```bash
    python manage.py migrate
    ```

6. **Run the Project:**

    ```bash
    daphne ocpp.asgi:application
    ```

    The APIs should now be accessible at `http://127.0.0.1:8000/`.

## Note

Redis or Memurai Must be Running:

1. **Start Redis or Memurai Server:**

    ```bash
    # for windows: windows key > search:services > find:memurai > start
    # Mac or linux use redis
    ```
