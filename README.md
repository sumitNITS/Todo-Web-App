This is a web based Todo-Web-App created using HTML, CSS, Python and django framework.

## How to use this Project In Local machine?

Great question, Follow the steps below:

Additionally, I've added the Dockerfile for this project too. Read till the end to know about how to run this project using docker container.

Software requirements for this project (For local machine): Git, Visual Studio Code (because it's cool), Docker Desktop

## Steps to Follow to run this Project in Local Machine

Clone the repository using: 

#git clone https://github.com/sumitNITS/Todo-Web-App.git

Install virtualenv for this project and activate it

#pip install virtualenv <br />
#python -m virtualenv <name_of_environment> <br />
#.\name_of_environment\Scripts\activate

Now, Move to the projec folder:

#cd Todo-Web-App

Install django framework for this project:

#pip install django

Migrate the components needed to run this project:

#python manage.py makemigrations <br />
#python manage.py migrate

Run the server locally using:

#python manage.py runserver

Cool, This project is now running in your localhost <br /> http://127.0.0.1:8000/

Cheers, we are done here!


## How to run this Project using Docker Container in Local Machine?

Make sure docker desktop is already installed and open in your system

Build an image from the Dockefile provided in this project using:

#docker build . -t todo-web-app

Check the image using the command:

#docker images

Copy the image_id_number and run the container using the docker image

#docker run -d -p 9000:9000 image_id_number

I'm using port 9000 for this project for docker container, verify the port in Dockerfile (You can change it and play along with the codes)

Cool, This project is now running in your localhost using docker container <br /> http://127.0.0.1:9000/
