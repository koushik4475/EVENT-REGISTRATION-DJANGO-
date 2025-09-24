# Django Event Registration System

A comprehensive event management web application built with Django that allows users to register for events and provides administrators with powerful tools to manage registrations.

-----

## 📸 Screenshots



### 🎯 Event Registration Form

<img width="1910" height="731" alt="Screenshot 2025-09-24 123745" src="https://github.com/user-attachments/assets/c6e7c37e-42a5-4987-a3ad-bf89fa5da884" />



### ✅ Event Registration Success Page

<img width="1919" height="298" alt="Screenshot 2025-09-24 123806" src="https://github.com/user-attachments/assets/16fffb71-e6b1-4e29-adf4-c8b2a13968ff" />

### ➕ Admin Panel - Adding Events

<img width="1916" height="637" alt="Screenshot 2025-09-24 123839" src="https://github.com/user-attachments/assets/250e8a8b-1028-4e8b-a2f6-be60402044e4" />


### 📋 Admin Panel - List of Events

<img width="1919" height="680" alt="Screenshot 2025-09-24 123917" src="https://github.com/user-attachments/assets/0c5eef75-228d-4fa6-8401-f91a48582cf6" />

### 📝 Admin Panel - Managing Registrations

<img width="1916" height="467" alt="Screenshot 2025-09-24 123945" src="https://github.com/user-attachments/assets/406bd9d7-e663-4d3b-bf31-1df02a9edf4f" />



### 🔐 Admin Login Page

<img width="1167" height="591" alt="Screenshot 2025-09-24 124010" src="https://github.com/user-attachments/assets/c62799b6-bba1-4396-8fdd-e94828ade68f" />




-----

## 🚀 Features

### User Features

  * **Event Registration:** Users can register for events by filling out a comprehensive form.
  * **Form Validation:** Robust form validation for fields like name, email, phone number, and event selection.
  * **Success Confirmation:** Users are redirected to a success page after a successful registration.
  * **Event Listing:** Browse available events and view event details.

### Admin Features

  * **Django Admin Panel:** A comprehensive admin interface for managing the entire system.
  * **Secure Authentication:** A secure login system for event organizers.
  * **Registration Management:**
      * View all registered participants.
      * **Approve, reject, or keep registrations pending.**
      * Edit user registration details.
      * Perform **bulk actions** for managing multiple registrations at once.
  * **Event Management:** Create, edit, and manage events directly through the admin panel.

-----

## 🛠️ Tech Stack

  * **Backend:** Django (Python)
  * **Frontend:** HTML, CSS, Bootstrap
  * **Database:** SQLite (default for development), PostgreSQL (for production)
  * **Version Control:** Git & GitHub

-----

## 📁 Project Structure

```
event-registration-system/
│
├── event_registration/   # Main Django project
│ ├── settings.py
│ ├── urls.py
│ └── wsgi.py
│
├── events/               # Django app
│ ├── models.py           # Event and Registration models
│ ├── views.py            # Class-based views
│ ├── forms.py            # Django forms
│ ├── admin.py            # Admin configuration
│ └── templates/          # HTML templates
│ ├── base.html
│ ├── registration_form.html
│ ├── success.html
│ └── event_list.html
│
├── static/               # CSS, JS, Images
├── requirements.txt      # Python dependencies
└── README.md
```

-----

## ⚙️ Installation & Setup

### Prerequisites

  * Python 3.8+
  * Git
  * `pip` (Python package manager)

### Local Development Setup

1.  **Clone the repository:**

    ```bash
    git clone https://github.com/yourusername/django-event-registration.git
    cd django-event-registration
    ```

2.  **Create a virtual environment:**

    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows: venv\Scripts\activate
    ```

3.  **Install dependencies:**

    ```bash
    pip install -r requirements.txt
    ```

4.  **Apply database migrations:**

    ```bash
    python manage.py makemigrations
    python manage.py migrate
    ```

5.  **Create a superuser (Admin):**

    ```bash
    python manage.py createsuperuser
    ```

6.  **Run the development server:**

    ```bash
    python manage.py runserver
    ```

### Access the Application

  * **Main site:** `http://127.0.0.1:8000/`
  * **Admin panel:** `http://127.0.0.1:8000/admin/`

-----

## 🖥️ Usage

### For Users

1.  Visit the homepage to see available events.
2.  Click on "Register" for any event.
3.  Fill out the registration form with your details.
4.  Submit and receive a confirmation on the success page.

### For Administrators

1.  Log in to the admin panel using your superuser credentials.
2.  Navigate to **Registrations** to manage participants.
3.  Change the registration status to:
      * **✅ Approved:** Confirm the registration.
      * **❌ Rejected:** Decline the registration.
      * **⏳ Pending:** Keep for review (default status).
4.  Manage events through the **Events** section to create, edit, or delete them.

-----

## 📊 Database Models

### `Event` Model

  * `event_name`
  * `description`
  * `date_and_time`
  * `location`
  * `maximum_capacity`

### `Registration` Model

  * `user_name`
  * `email_address`
  * `phone_number`
  * `selected_event` (ForeignKey)
  * `registration_status` (Pending/Approved/Rejected)
  * `timestamp`

-----

## 🌟 Key Technical Features

  * **Django Class-Based Views** (`ListView`, `CreateView`) for efficient, reusable code.
  * **Form handling** with built-in validation.
  * **Database relationships** using `ForeignKey` to link registrations to events.
  * **Django Admin customization** for a powerful backend interface.
  * **Bootstrap** for a responsive, mobile-friendly design.
  * **`reverse_lazy()`** for clean redirection after form submission.
  * **Git** for version control and collaborative development.

-----

## 🚀 Deployment

This application is ready for deployment on platforms that support Django, such as:

  * Heroku
  * DigitalOcean
  * AWS EC2
  * PythonAnywhere

-----

## 🤝 Contributing

Contributions are welcome\! Please feel free to submit a Pull Request.

-----

## 📄 License

This project is open-source and available under the **MIT License**.

-----

## 📞 Contact

For any questions or collaboration opportunities, feel free to contact me.

**Koushik H Y**

  * **Email:** koushik4475@gmail.com
  * **Portfolio:** [https://koushik4475.netlify.app](https://koushik4475.netlify.app)

-----

Built with ❤️ by Koushik H Y | Full Stack Developer

⭐ If you found this project helpful, please give it a star on GitHub\!
