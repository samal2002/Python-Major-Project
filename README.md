MealMate - Online Food Ordering System

MealMate is a Django-based web application that allows users to register as restaurant owners or customers. Restaurant owners can manage their restaurants, while customers can browse menus, place orders, and make secure payments using Razorpay.

🚀 Features

🔐 Authentication

User registration and login for both restaurant owners and customers

Secure authentication using Django's built-in authentication system

🍽️ Restaurant Management (For Owners)

Add new restaurants

Edit and update restaurant details

Delete restaurants

🛒 Menu & Orders (For Customers)

Browse restaurant menus

Add items to the cart

Place orders

💳 Payment Integration

Razorpay integrated for secure online payments

📌 Installation & Setup

1️⃣ Clone the Repository

git clone https://github.com/your-username/mealmate.git
cd mealmate

2️⃣ Set Up a Virtual Environment

python3 -m venv venv
source venv/bin/activate  # For Mac/Linux
venv\Scripts\activate  # For Windows

3️⃣ Install Dependencies

pip install -r requirements.txt

4️⃣ Apply Migrations

python manage.py migrate

5️⃣ Create a Superuser (For Admin Access)

python manage.py createsuperuser

6️⃣ Run the Development Server

python manage.py runserver

Now, open your browser and go to: http://127.0.0.1:8000/

📂 Directory Structure (After Commit)

mealmate/
│── delivery/
│   │── migrations/
│   │── static/
│   │── templates/delivery/
│   │   ├── add_res.html
│   │   ├── base.html
│   │   ├── checkout.html
│   │   ├── cusmenu.html
│   │   ├── customer_home.html
│   │   ├── display_res.html
│   │   ├── failed.html
│   │   ├── index.html
│   │   ├── menu.html
│   │   ├── orders.html
│   │   ├── show_cart.html
│   │   ├── sign_in.html
│   │   ├── sign_up.html
│   │   ├── success.html
│   │   ├── userdata.html
│   │── __init__.py
│   │── admin.py
│   │── apps.py
│   │── forms.py
│   │── models.py
│   │── tests.py
│   │── views.py
│── manage.py
│── requirements.txt
│── .gitignore
│── README.md

📡 API Endpoints (If Using Django REST Framework)

Method

Endpoint

Description

GET

/restaurants/

List all restaurants

POST

/restaurants/add/

Add a new restaurant

PUT

/restaurants/update/<id>/

Update restaurant details

DELETE

/restaurants/delete/<id>/

Delete a restaurant

GET

/menu/

Get menu items

POST

/order/

Place an order

💳 Razorpay Payment Integration

Sign up at Razorpay and get API keys from the Razorpay Dashboard.

Add API keys to Django settings:

RAZORPAY_KEY_ID = "your_key_id"
RAZORPAY_KEY_SECRET = "your_key_secret"

🎯 Contributing

We welcome contributions! If you want to improve MealMate, feel free to:

Fork the repository

Create a new branch (git checkout -b feature-branch)

Commit your changes (git commit -m 'Add new feature')

Push to your branch (git push origin feature-branch)

Create a pull request

📜 License

This project is licensed under the MIT License.

📬 Contact

For any queries or suggestions, feel free to reach out:
📧 Email: your-email@example.com🌐 GitHub: your-username
