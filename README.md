# E-commerce Website

An e-commerce platform built with Django that allows users to browse products, add them to a cart, and proceed with checkout.

## Features
- User authentication (registration, login, logout)
- Product listing with search and filters
- Shopping cart functionality
- Order management for users
- Admin panel for managing products, categories, and orders

## Technologies Used
- **Django:** The web framework used to build the project
- **SQLite:** Default database for development (can be replaced with PostgreSQL, MySQL, etc.)
- **Bootstrap:** For responsive design and styling
- **Stripe:** Payment gateway integration

## Installation

### Prerequisites
- Python 3.13
- Django 4.1.2 or higher
- Virtual environment (recommended)

### Steps
1. Clone the repository:
    ```sh
    git clone https://github.com/abhishektotre/ecommerce.git
    cd ecommerce
    ```

2. Create a virtual environment and activate it:
    ```sh
    python -m venv venv
    source venv/bin/activate   # On Windows use `venv\Scripts\activate`
    ```

3. Install the required dependencies:
    ```sh
    pip install -r requirements.txt
    ```

4. Apply the database migrations:
    ```sh
    python manage.py migrate
    ```

5. Create a superuser for the admin panel:
    ```sh
    python manage.py createsuperuser
    ```

6. Run the development server:
    ```sh
    python manage.py runserver
    ```

7. Access the application at `http://127.0.0.1:8000/` and the admin panel at `http://127.0.0.1:8000/admin/`.

## Configuration

### Environment Variables
Create a `.env` file at the root of your project to store sensitive information such as the secret key and database credentials. Here's an example:
SECRET_KEY=your_secret_key DEBUG=True DATABASE_URL=sqlite:///db.sqlite3 STRIPE_PUBLIC_KEY=your_stripe_public_key STRIPE_SECRET_KEY=your_stripe_secret_key

## Usage
- **Admin Panel:** Manage products, categories, and orders.
- **Product Listing:** Browse and search for products.
- **Shopping Cart:** Add products to the cart and proceed with checkout.
- **Order Management:** View order history and details.

## Contributing
Contributions are welcome! Please fork the repository and create a pull request with your changes.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more information.

## Acknowledgments
- [Django Documentation](https://docs.djangoproject.com/)
- [Bootstrap Documentation](https://getbootstrap.com/)
- [Stripe Documentation](https://stripe.com/docs)

