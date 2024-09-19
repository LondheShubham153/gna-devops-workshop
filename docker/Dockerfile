# Pulling base image 
FROM python:3.9

# working directory to run stuff
WORKDIR /devops

RUN apt-get update -y && apt-get install git -y 

# Get the project source code
RUN git clone https://github.com/LondheShubham153/django-notes-app.git


# install required packages
RUN pip install -r django-notes-app/requirements.txt

# exposing the port where app runs
EXPOSE 8080

# Run the app
CMD ["python","django-notes-app/manage.py","runserver","0.0.0.0:8080"]
