# Python-Flask-Notes

1) Open vs code in the project folder and run pip install flask to install python flask.
2) Create app.py where all the rest apis will be defined and all routes will be managed.
3) Install flask sqlalchemy and import the required packages.
4) Create a class and inherit db.model into that class. The schema of the table will be defined in this class.
5) Create repr method which will be called when object of that class is printed.
6) Establish the database connection by writing the necessary lines of code. This can be taken from flask sqlalchemy documentation.
7) Always remember to add - app.app_context().push() which will allow you to push the database from your app.
8) Type python in another terminal. Type from app import db and then type db.create_all(). This will create the database. You will observe that a folder called instance is automatically created and inside the folder your db will be present.
9) Create a folder called "template" in which you can add all your HTML files.
10) Create a file named "layout.html" in the template folder which will contain code that is common to all the HTML files such as external links- bootstrap css & js, title section as well as the navbar.
11) This template will be inherited by other html files so that you can reuse the existing code and also avoid writing the same code again and again.
12) Template inheritance can be performed with the help of jinja2 template which is an extension in vs code and can be downloaded from extension section.
13) If your route has a method which will accept both "Get" as well as "Post" request, then remember to add methods=["GET","POST"] to the route else the post request would not get accepted.
