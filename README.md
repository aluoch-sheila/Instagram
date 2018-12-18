# Instagram
 A  a clone of the image sharing network, Instagram. Users can sign up login, view and post photos and follow other users.
## Built By [Aluoch Sheila](https://github.com/aluoch-sheila/Instagram.git)

## Description
This is an application that allows users to view images. Image details are stored in categories and tagged by Location. The admin is responsible for uploading, editing or deleting images.

## User Stories
These are the behaviours/features that the application implements for use by a user.

Users would like to:
* Register and Sign in to the application.
* Upload my pictures to the application.
* See my profile with all my pictures.
* Follow other users and see their pictures on my timeline.
* Like or Save a picture and leave a comment on it.

# Setup and installation

## Admin Abilities
These are the behaviours/features that the application implements for use by the admin.

Admin should:
* Sign in to the Instazone
* Create new images for showcasing
* Delete images
* Update image post details.


## Specifications
| Behaviour | Input | Output |
| :---------------- | :---------------: | ------------------: |
| Display  images | **Home page** | Clickable links to open any images in a modal |
| Display single images on click | **On  signup** | All details should be viewed|
| To add an image  | **Through Admin dashboard** |  add  Image|
| To search  | **Enter text in search bar** | Users can search by category|


## SetUp / Installation Requirements
### Prerequisites
* python3.6
* pip
* virtualenv
* Requirements.txt

### Cloning
* git clone https://github.com/aluoch-sheila/Instagram.git
cd Instagram
Activate virtual environment

create and acvite a virtual environment python3.6 -m venv virtual && source virtual/bin/activate

Install dependancies

Install dependancies that will create an environment for the app to run pip install -r requirements.txt

Create the Database

- psql
- CREATE DATABASE instazone;
.env file

Create .env file and paste paste the following filling where appropriate:

SECRET_KEY = '<Secret_key>'
DBNAME = 'insta'
USER = '<Username>'
PASSWORD = '<password>'
DEBUG = True
Run initial Migration

python3.6 manage.py makemigrations instazone
python3.6 manage.py migrate
Run the app

## Running the Application
* Creating the virtual environment

        $ python3.6 -m venv --without-pip virtual
        $ source virtual/bin/activate
        $ curl https://bootstrap.pypa.io/get-pip.py | python

* Installing Django and other Modules

        $ see Requirements.txt

* To run the application, in your terminal:

        $ python3.6 manage.py runserver

## Testing the Application
* To run the tests for the class files:

        $ python3.6 manage.py test images

## Technologies Used
* Python3. /Django
* postgresql
* Bootstrap4

