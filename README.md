
#  REST API for Product Resource Management
This project is based on building a simple API in python which uses Flask framework to manage products.The API allows the user to create products and retrieve a list of all the products.
## Requirements
- Python 3.12.6
- Flask (`pip install Flask`)  This is the REST API framework I used
- Requests library for client interaction (`pip install requests`)

## Setup Instructions

### 1. Set up the environment
- Installed Python 3.12.6 and pip if not already installed.
- Created a virtual environment :
    ```gitbash
    python -m venv .venv
    
    .\.venv\Scripts\Activate.ps1    # For Windows Powershell

     .\.venv\Scripts\activate.bat   # For Windows CMD

    ```
- Install the python webframework :
    ```bash
    pip install Flask
    ```

### 2. Run the API Server
- Navigate to the Product_Resource folder containing the `api.py` script.
- Run the API:
    ```bash
    python api.py
    ```
  This will start an API server at `http://127.0.0.1:5000`.

### 3. Test the API Endpoints
Use the Python script `client.py` to interact with the API.
- Ensure you have established a connection to the server 
- To add new products:
    ```bash
    python client.py
    ```

This will create two products and print the list of all products.

### Manual Testing with cURL :
-Installed  cURL   
  I used the tool cURL  to interact with the API endpoints.

**POST /products Example** (create a product):
```bash
curl -X POST http://127.0.0.1:5000/products \
-H "Content-Type: application/json" \
-d '{"name": "Laptop", "description": "High-Performance and good storage", "price": 25000}'


![Product Image](Product_Resource/README.md/Images/image1.png)
![Product Image](Product_Resource/README.md/Images/image2.png)
