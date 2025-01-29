# Pyshop - Django Product Catalog

A simple product catalog system built with Django.

## Features
- Product listing page
- Product detail pages
- Add to Cart functionality
- Admin management interface

## Prerequisites

- Python 3.8+
- pip
- Git
- Virtual Environment (recommended)

## Installation

### 1. Clone the repository
```bash
git clone https://github.com/saidulislam2003/Pyshop.git
cd Pyshop
```

### 2. Create and activate virtual environment
```bash
python -m venv venv
# Windows:
venv\Scripts\activate
# Linux/MacOS:
source venv/bin/activate
```

### 3. Install dependencies
```bash
pip install -r requirements.txt
```

### 4. Configure environment variables
Create a `.env` file in the project root:
```python
SECRET_KEY=your-secret-key-here
DEBUG=True
```

Generate a secret key with:
```bash
python -c 'from django.core.management.utils import get_random_secret_key; print(get_random_secret_key())'
```

### 5. Run migrations
```bash
python manage.py migrate
```

### 6. Create admin user
```bash
python manage.py createsuperuser
```

### 7. Run development server
```bash
python manage.py runserver
```

## Accessing the Project

- Product listing: http://localhost:8000/products/
- Admin panel: http://localhost:8000/admin/

## Project Structure

```
Pyshop/
├── products/           # Contains all product functionality
│   ├── migrations/
│   ├── templates/
│   ├── admin.py
│   ├── models.py
│   ├── views.py
│   └── ...
├── manage.py
└── pyshop/             # Project configuration
    ├── settings.py
    ├── urls.py
    └── ...
```

## Adding Products
1. Access the admin panel at http://localhost:8000/admin/
2. Log in with your superuser credentials
3. Add products through the admin interface

## Usage
- Browse products at http://localhost:8000/products/
- Click "Add to Cart" to add products to your cart
- Prices are displayed in USD ($)

## License
MIT License - see [LICENSE](LICENSE) for details


