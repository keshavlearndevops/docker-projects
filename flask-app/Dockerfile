# base image, it will pull the python image from the DockerHub
FROM python:3.9

# setting Working directory for app
WORKDIR app/

#copy code from system to container
COPY app.py .

# install required libraries
# RUN is used while Container creation 
RUN pip install flask

#run the application
# CMD is used to run a command POST container creation
CMD ["python","app.py"]                     
