# 🎓 Online Course Assessment Platform

![Django](https://img.shields.io/badge/Django-092E20?style=for-the-badge&logo=django&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Bootstrap](https://img.shields.io/badge/Bootstrap-563D7C?style=for-the-badge&logo=bootstrap&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-07405E?style=for-the-badge&logo=sqlite&logoColor=white)

A modern, visually stunning online learning management system where users can enroll in courses, study lessons, and take final assessments to earn their grades.

---

## ✨ Key Features

*   **Modern UI/UX**: Premium glassmorphism design, vibrant gradients, and smooth hover animations applied across all pages.
*   **Course Management**: Browse available courses, view details, and enroll with a single click.
*   **User Authentication**: Secure registration and login system with beautifully styled, centered forms.
*   **Assessment Engine**: Take dynamic exams directly from the course page.
*   **Automated Grading**: Instant calculation of exam scores with clear pass/fail visual feedback and detailed answer breakdown.
*   **Django Admin Integration**: Fully configured backend to quickly manage courses, lessons, questions, and choices.

## 🚀 Getting Started

### Prerequisites

*   Python 3.8+
*   pip (Python package installer)

### Installation

1.  **Clone the repository** (if you haven't already):
    ```bash
    git clone https://github.com/ibm-developer-skills-network/final-cloud-app-with-database.git
    cd final-cloud-app-with-database
    ```

2.  **Install the dependencies**:
    ```bash
    pip install -r requirements.txt
    ```

3.  **Apply database migrations**:
    ```bash
    python manage.py makemigrations
    python manage.py migrate
    ```

4.  **Create a superuser** (for accessing the Django Admin panel):
    ```bash
    python manage.py createsuperuser
    ```

5.  **Run the development server**:
    ```bash
    python manage.py runserver
    ```

6.  Open your browser and navigate to: `http://127.0.0.1:8000/`

---

## 🏗️ Architecture & Database

This project extends the base `onlinecourse` application by adding a robust assessment feature.

### Entity-Relationship Diagram (ERD)

The following diagram illustrates the database architecture, specifically highlighting the relationship between Courses, Enrollments, Submissions, Questions, and Choices.

![Onlinecourse ER Diagram](https://github.com/ibm-developer-skills-network/final-cloud-app-with-database/blob/master/static/media/course_images/onlinecourse_app_er.png)

*   **Question**: Linked to a specific `Course`.
*   **Choice**: Linked to a specific `Question`. Marked as correct/incorrect.
*   **Submission**: Linked to an `Enrollment` (User + Course) and tracks the selected `Choice`s.

---

## 🎨 Design Highlights

The frontend has been completely overhauled to provide a premium feel:
*   **Glassmorphism**: Translucent navbars and slightly transparent application cards.
*   **Responsive Grid**: Clean layout utilizing the Bootstrap grid system.
*   **Custom CSS Variables**: Easy theming through `style.css` using modern CSS properties.

---
*Developed as the final project for the IBM Cloud App with Database specialization.*
