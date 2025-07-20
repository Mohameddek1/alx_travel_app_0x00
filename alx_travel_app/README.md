# alx\_travel\_app\_0x00

> **A travel booking API** built with Django and Django REST Framework (DRF).

This project is a duplicate of `alx_travel_app`, extended for database modeling and data seeding. It features models for Listings, Bookings, and Reviews and includes a management command to populate sample data.

---

## Features

* **Django Models**:

  * `Listing`: Represents travel listings with destination, description, price, and availability.
  * `Booking`: User reservations for listings, including check-in and check-out dates.
  * `Review`: User-submitted reviews on listings with ratings.

* **DRF Serializers**:

  * `ListingSerializer`
  * `BookingSerializer`

* **Database Seeder**:

  * Populates the database with sample `Listing` entries using a custom Django management command.

---

## Project Structure

```bash
alx_travel_app_0x00/
├── alx_travel_app/
│   ├── __init__.py
│   ├── settings.py
│   ├── urls.py
│   └── wsgi.py
├── listings/
│   ├── __init__.py
│   ├── admin.py
│   ├── apps.py
│   ├── models.py        # Listing, Booking, Review models
│   ├── serializers.py   # ListingSerializer, BookingSerializer
│   ├── views.py
│   ├── urls.py
│   └── management/
│       └── commands/
│           └── seed.py  # Seeder command
├── manage.py
└── README.md
```

---

## Setup Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/alx_travel_app_0x00.git
cd alx_travel_app_0x00
```

### 2. Create and Activate Virtual Environment

```bash
python3 -m venv venv
source venv/bin/activate
```

### 3. Install Requirements

```bash
pip install -r requirements.txt
```

### 4. Apply Migrations

```bash
python manage.py makemigrations
python manage.py migrate
```

### 5. Run Seeder

```bash
python manage.py seed
```

### 6. Run the Development Server

```bash
python manage.py runserver
```

---

## API Endpoints (Example)

* `/api/listings/`: List all travel listings
* `/api/bookings/`: Create or view bookings
* `/api/reviews/`: Submit and view reviews

---

## Author

Mohameddeq Ahmed
ALX Backend Student

---

## License

This project is part of the **ALX Software Engineering Program** and is licensed for educational use.
