# Wagtail experiments

A sandbox for getting to know the Wagtail CMS. 

## Getting up and running

You'll need a couple of dependencies before getting started `libjpeg` and `zlib`. See the ['Getting started' on the Wagtail docs](https://docs.wagtail.io/en/stable/getting_started/tutorial.html) for installation instructions.

Once you've got these you should be able to get going with these commands: 

Use these steps to get up and running. See also the general Python advice for additional tips.

* Ensure you have Python 3.6 or greater and pip installed
* Clone this repository
* Create a virtual environment with `python3 -m venv mysite/env`
* From the root directory run `source mysite/env/bin/activate`
* Upgrade pip with `pip install --upgrade pip`
* Install dependencies with `pip install wagtail`
* Start the application with `wagtail start mysite mysite`

The `start` command we've just used **generates a new mysite folder** with a few Wagtail-specific extras, including the required project settings, a “home” app with a blank HomePage model and basic templates, and a sample “search” app.

* Enter the new site with `cd mysite`
* Install dependencies with `pip install -r requirements.txt`
* Migrate the database with `python manage.py migrate` (by default this will be a SQLite database)
* Create an admin super user with `python manage.py createsuperuser`
* Start the server with `python manage.py runserver`

You can now access: 

* The site from http://127.0.0.1:8000/
* The admin interface from http://127.0.0.1:8000/admin