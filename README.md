# Dosa Orders Project

Welcome to the **Dosa Orders Project**! This is a Python script that helps a restaurant organize its orders into two easy-to-read JSON files: one for customer information and one for the items ordered. Let’s break it down!

## Project Overview

The script reads an orders JSON file and then generates two new JSON files:

1. **customers.json**: Contains customer phone numbers and their names.
2. **items.json**: Contains the menu items, their prices, and how many times they've been ordered.

### Outputs Example:

- **customers.json**:
    ```json
    {
        "732-555-5509": "Damodhar",
        "609-555-0124": "Karl"
    }
    ```
- **items.json**:
    ```json
    {
        "Cheese Madurai Masala Dosa": {
            "price": 13.95,
            "orders": 10
        },
        "Onion Chilli Masala Dosa": {
            "price": 11.95,
            "orders": 5
        }
    }
    ```

## How to Get Started

### Prerequisites

Before you run this, make sure you have:

- **Python 3.x** installed on your system.
- An orders JSON file structured like this:

    ```json
    [
        {
            "timestamp": 1702219784,
            "name": "Damodhar",
            "phone": "732-555-5509",
            "items": [
                {
                    "name": "Cheese Madurai Masala Dosa",
                    "price": 13.95
                }
            ],
            "notes": "extra spicy"
        }
    ]
    ```

### Running the Project

1. **Clone the Repository**: First, you’ll want to clone the repository to your local machine:
    ```bash
    git clone https://github.com/your-username/dosa-orders-project.git
    cd dosa-orders-project
    ```

2. **Run the Script**: Once inside the project folder, run the Python script with your orders file:
    ```bash
    python dosa_orders.py example_orders.json
    ```

3. **View the Results**: After running the script, you should see two new JSON files:
    - `customers.json`: This file contains the customers' phone numbers and names.
    - `items.json`: This file contains item names, prices, and the number of times each item was ordered.

## Contributing
If you have suggestions for improvement, feel free to fork this repo, make changes, and submit a pull request! All contributions are welcome.

