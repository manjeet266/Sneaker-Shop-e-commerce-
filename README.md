# Sneaker Shop E-Commerce Platform

![Sneaker Shop Banner](main/static/images/jumbotron.jpg)

A fully functional, custom-built e-commerce web application for a sneaker shop. This project is built using Python and the Django framework, providing a robust backend and an intuitive frontend for browsing, managing a shopping cart, and checking out.

## Features

- **Product Catalog:** Browse through different sneaker brands, models, colors, and sizes.
- **Inventory Management:** Automatically tracks quantities and inventory of different shoe sizes and colors.
- **Shopping Cart:** Add, update, and remove items from the shopping cart seamlessly.
- **User Accounts & Authentication:** Secure user registration, login, and profile management (with `bcrypt` for password hashing).
- **Checkout Process:** Complete order checkout, including managing shipping addresses and saving credit card details securely.
- **Order History:** Users can view their past orders and track their status.
- **Admin Management:** Backend interface to easily add new brands, shoes, and update inventory.

## Technologies Used

- **Backend:** Python, Django 2.2.4
- **Database:** SQLite3 (default)
- **Frontend:** HTML, CSS, Django Templates
- **Image Handling:** Pillow (for rendering product galleries and images)

## Project Structure

```
sneaker-shop-master/
│
├── main/                   # Core Django application containing views, models, and URLs
│   ├── templates/          # HTML templates (home, cart, checkout, admin, etc.)
│   ├── static/             # CSS files, icons, and static product images
│   ├── models.py           # Database models (User, Shoe, Cart, Order, etc.)
│   └── views.py            # Business logic and request handling
│
├── sneaker_shop/           # Django project configuration settings
│
├── media/gallery/          # User-uploaded or dynamic product images
│
├── requirements.txt        # Python dependencies
└── manage.py               # Django execution script
```

## Setup & Installation

Follow these steps to run the application locally on your machine.

**1. Clone the repository**
```bash
git clone https://github.com/manjeet266/Sneaker-Shop-e-commerce-.git
cd Sneaker-Shop-e-commerce-
```

**2. Create a virtual environment (Recommended)**
```bash
python -m venv venv
```

**3. Activate the virtual environment**
- On Windows:
  ```bash
  venv\Scripts\activate
  ```
- On macOS/Linux:
  ```bash
  source venv/bin/activate
  ```

**4. Install Dependencies**
```bash
pip install -r requirements.txt
```

**5. Apply Database Migrations**
```bash
python manage.py makemigrations
python manage.py migrate
```

**6. Run the Development Server**
```bash
python manage.py runserver
```

Open your browser and navigate to `http://127.0.0.1:8000/` to view the application!

## Contributing

Feel free to fork the repository and submit pull requests to contribute to this project. For major changes, please open an issue first to discuss what you would like to change.
