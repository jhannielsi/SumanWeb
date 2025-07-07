# SumanWeb
Suman Company Website
This is a Flask-based backend for the Suman Company website, serving static HTML pages and handling a contact form submission.Table of ContentsAbout the ProjectFeaturesProject StructureGetting StartedPrerequisitesInstallationRunning the ApplicationFrontend FilesFuture EnhancementsContactAbout the ProjectThis project provides the backend infrastructure for the Suman Company website. It uses Flask to serve various static HTML pages (Home, Introduction, Products, Solutions, Customer, Contact) and includes basic logic for handling contact form submissions and displaying dynamic news content.FeaturesStatic Page Serving: Renders pre-built HTML pages for different sections of the website.Contact Form Handling: Processes form submissions from the "Contact Us" page, logging the data to the console and providing user feedback via flash messages.Dynamic News Section: Demonstrates how to pass dynamic data (news articles) from the Flask backend to an HTML template.Static File Management: Correctly serves CSS and image assets.Responsive Design: (Inherited from frontend) The frontend is designed to be responsive across various devices.Project Structureyour_project_name/
├── app.py                      # Main Flask application file
├── static/
│   ├── css/
│   │   └── style.css           # Global CSS styles
│   └── images/
│       ├── bg.png              # Background image for hero section
│       ├── product1.png        # Placeholder product image
│       ├── product2.png        # Placeholder product image
│       └── suman logo.png      # Company logo / Favicon
└── templates/
    ├── contact.html            # Contact Us page
    ├── customer.html           # Customer page
    ├── index.html              # Home page
    ├── introduction.html       # Company Introduction page
    ├── products.html           # Products page
    ├── solutions.html          # Solutions page
    └── news.html               # News page (dynamic content)
Getting StartedTo get a local copy up and running, follow these simple steps.PrerequisitesPython 3.8+pip (Python package installer)InstallationClone the repository (if applicable) or set up your project directory:If you're starting from scratch, create the your_project_name directory and place app.py, static/, and templates/ inside it as described in the Project Structure.Navigate into your project directory:cd your_project_name
Create a Python virtual environment (recommended):python -m venv venv
Activate the virtual environment:On macOS/Linux:source venv/bin/activate
On Windows:venv\Scripts\activate
Install Flask:pip install Flask
Running the ApplicationEnsure your virtual environment is activated.Run the Flask application:flask run
Alternatively, you can run:python app.py
Access the application:Open your web browser and navigate to: http://127.0.0.1:5000The console where you ran flask run will display messages, including contact form submissions.Frontend FilesThe project utilizes the following HTML and CSS files for the frontend:templates/index.html: The main landing page.templates/introduction.html: Details about the company.templates/products.html: Information about products.templates/solutions.html: Details on company solutions.templates/customer.html: Customer information.templates/contact.html: Contact form for inquiries.templates/news.html: Displays dynamic news articles fetched from the backend.static/css/style.css: Contains the global styling for the website.static/images/: Contains various image assets used throughout the site.Future EnhancementsDatabase Integration: Replace the in-memory news_articles list with a proper database (e.g., SQLite, PostgreSQL) using Flask-SQLAlchemy or Flask-SQLModel.Email Sending: Implement actual email sending for contact form submissions (e.g., using Flask-Mail or a direct SMTP library).Form Validation: Add server-side validation for contact form fields to ensure data integrity and security.Admin Panel: Create a simple admin interface to manage news articles, contact inquiries, etc.User Authentication: If needed, add user login/registration functionality.Error Pages: Implement custom 404 (Not Found) and 500 (Internal Server Error) pages.ContactFor any questions or suggestions, please reach out.
