# tanX Assignment

## Description
This project analyzes data from an online store to compute various revenue metrics. The main program (`main.py`) reads data from `orders.csv` and performs tasks such as computing monthly revenue, product revenue, customer revenue, and identifying top customers.

## How to Run
1. **Install Docker:**
    - Ensure you have Docker installed on your machine. Follow the instructions based on your operating system:
        - [Install Docker on Windows](https://docs.docker.com/desktop/install/windows-install/)
        - [Install Docker on macOS](https://docs.docker.com/desktop/install/mac-install/)
        - [Install Docker on Linux](https://docs.docker.com/desktop/install/linux-install/)

2. **Clone this repository:**
    ```bash
    git clone https://github.com/BhanuSandeepVellalacheruvu/tanX
    ```

3. **Navigate to the project directory:**
    ```bash
    cd tanX
    ```

4. **Run the Main Program:**
    - Replace `app/orders` in `app/main.py` with the actual file path for your data.
    - Execute the following command to build and run the main program:
        ```bash
        docker-compose up task
        ```

5. **Run Tests:**
    - Execute the following command to build and run the tests:
        ```bash
        docker-compose up test
        ```

[Test Output](https://github.com/BhanuSandeepVellalacheruvu/tanX/assets/118993028/b29b4ebf-ae79-498b-b421-2bfea0077e89)

## Providing Input
- The main program reads data from `orders.csv`. Ensure that you have a CSV file with the required columns (`order_id`, `customer_id`, `order_date`, `product_id`, `product_name`, `product_price`, `quantity`).

- If you want to use a different data file or provide custom input, replace the file path in `app/main.py` accordingly.

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

## Interacting with the Application

### Input Declaration:
- The main program reads input data from a CSV file named `orders.csv`.
- To customize input or use a different data file, modify the `app/orders.csv` variable in `app/main.py`.

### Providing Input:
1. Ensure your data file follows the required structure with columns: `order_id`, `customer_id`, `order_date`, `product_id`, `product_name`, `product_price`, `quantity`.
2. Replace `app/orders.csv` in `app/main.py` with the actual path to your data file.
3. Save the changes.
4. Run the main program using:
    ```bash
    docker-compose up task
    ```

## Example: Using orders.csv
- The repository includes a sample data file named `orders.csv` in the `app/` directory.
- This file serves as an example input for the main program.
- To run the main program with the provided example, ensure `app/orders.csv` is set to `'orders.csv'` in `app/main.py`.
- Execute the following command:
    ```bash
    docker-compose up task
    ```
## Viewing Results

### Main Program Output:
- The main program will display the computed metrics, such as monthly revenue, product revenue, customer revenue, and top customers, in the console.

### Test Results:
- The test results will be displayed in the console, showing whether the tests passed or if there are any failures.

## Customizing Dockerized Application

### Docker Configuration:
- The Docker configuration is defined in the `Dockerfile` and `docker-compose.yml` files.

### Dependencies:
- Python dependencies are listed in the `requirements.txt` file.

### Cleaning Up:
- After running the application or tests, you can clean up the Docker containers using:
    ```bash
    docker-compose down

### Detached Mode:
- If you prefer to run the Dockerized application in the background (detached mode), use the `-d` flag:
    ```bash
    docker-compose up -d task
    ```

## Dockerized Application
The application is containerized using Docker for easy deployment. Docker Compose manages the services and dependencies.
