# Django JWT Authentication

This project demonstrates how to implement authentication in a Django application using JSON Web Tokens (JWT).

## Features

- User registration
- User login with JWT token generation
- JWT token-based authentication for accessing protected routes
- Token refreshing and token verification

## Requirements

- Python 3.x
- Django 3.x or later
- djangorestframework
- djangorestframework-simplejwt

## Installation

1. **Clone the repository**:
    ```bash
    git clone https://github.com/Clifford537/kazi_conn_backend.git
    cd kazi_conn_backend
    ```

2. **Create a virtual environment**:
    ```bash
    python3 -m venv venv
    source venv/bin/activate
    ```

3. **Install the dependencies**:
    ```bash
    pip install -r requirements.txt
    ```

4. **Apply migrations**:
    ```bash
    cd KaziConn
    python manage.py migrate
    ```

5. **Run the development server**:
    ```bash
    python manage.py runserver
    ```
    
6. **To test the api run the command**:
      ```bash
    python manage.py runserver
    ```

## Usage

### Registration

To register a new user, send a POST request to the `http://127.0.0.1:8000/user_account/api/users/create/` endpoint with the following JSON payload:

```json
{
    "email":   "This field may not be blank.",
    "userName": "This field may not be blank.",
    "firstName": "This field may not be blank.",
    "lastName": "This field may not be blank."
    and other fields
}

