# tanX Assignment

## Description
This project analyzes data from an online store to compute various revenue metrics. The main program (`main.py`) reads data from `orders.csv` and performs tasks such as computing monthly revenue, product revenue, customer revenue, and identifying top customers.

## How to Run
1. Ensure you have Docker installed on your machine.

2. Clone this repository:
    ```bash
    git clone https://github.com/BhanuSandeepVellalacheruvu/tanX
    ```

3. Navigate to the project directory:
    ```bash
    cd tanX
    ```

4. **Run the Main Program:**
    - Replace `your_csv_file_path` in `app/main.py` with the actual file path for your data.
    - Execute the following command to run the main program:
        ```bash
        docker-compose up task
        ```

5. **Run Tests:**
    - Execute the following command to run the tests:
        ```bash
        docker-compose up test
        ```

## Project Structure
The project has the following structure:

- **app/**
  - `main.py`: The main Python program for online store analytics.
  - `orders.csv`: Sample data file.

- **tests/**
  - `test_main.py`: Test file for the main program.
  - `test_orders.csv`: Test data file (if needed).

- `Dockerfile`: Dockerfile for the application.
- `docker-compose.yml`: Docker Compose file for services.
- `README.md`: This file with instructions.
- `requirements.txt`: Python dependencies file.

## Dockerized Application
The application is Dockerized for easy deployment. Docker Compose is used to manage the services.
