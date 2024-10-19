Best-Performing Student Recognition System
Project Overview
The Best-Performing Student Recognition System is a web application built using Flask that identifies and displays the top-performing students based on various performance metrics. It provides users with the ability to view top students by admission year and offers detailed insights into individual student performances. The application leverages a machine learning model (Random Forest Regressor) to predict student performance scores based on available features in the dataset.

Key Features
Home Page:

Displays a welcoming heading: "Best-Performing Student Recognition System."
Provides buttons for each available year of admission.
Buttons are laid out side-by-side with appropriate spacing for improved UI.
Top Performing Students by Year:

On selecting a specific year, the system navigates to a page showing the top 3 students for that year.
Each student entry displays their name, student ID, and predicted performance score.
A "Details" button is available for each student to view all additional information (like grades, admission year, etc.).
Show All Results:

A button on the home page allows users to view the top 3 students across all available years.
Displays a consolidated list of top-performing students with sorting and pagination support.
CSV/Excel Export:
Export student results as CSV files for reporting or further analysis


Technologies Used
Backend:
Flask (Python web framework)
Flask-Restful for API integration (optional)
Flask-Login for user authentication (optional)

Machine Learning:
Random Forest Regressor (using scikit-learn)
Frontend:
HTML5, CSS3, JavaScript

Key Dependencies:

Flask
scikit-learn
pandas
Flask-Login (for authentication)
Flask-Paginate (for pagination)
Chart.js (for visualizations)
Dataset Preparation

Place your student dataset (student_dataset1.csv) in the project directory. The dataset should contain columns such as Name, Student_id, Admitted_year, Core_Course_1_Grade, Overall_Score, etc.
The application uses this dataset for student ranking and performance prediction.
Usage

Navigate to the home page to select a specific year and view top-performing students or use the "Show all Results" button to view the top 3 performers from all years.
Click on "Details" to view detailed student performance information.

Best-Performing Student Recognition System/
│
├── app.py                      # Flask backend application
├── student_dataset1.csv         # Sample dataset for students
├── templates/
│   ├── index.html               # Home page template
│   ├── results.html             # Results page template for top-performing students
│   ├── student_details.html     # Template for individual student details
│   └── all_results.html         # Displays the top 3 students for all years
├── static/
│   ├── style.css                # Custom CSS for styling the pages
│   
├── requirements.txt             # Python dependencies
└── README.md                    # Project description and instructions
