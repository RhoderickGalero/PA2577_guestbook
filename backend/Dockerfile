# pull official base image
FROM python:3.7

# set work directory
RUN mkdir /app
WORKDIR /app
# copy files/directories
ADD . /app/

# install dependencies
RUN pip install -r requirements.txt

# set environment variables
ENV DATABASE_URI="localhost"
ENV FLASK_APP=main.py

EXPOSE 5000

# launch the app 
CMD ["python", "/app/main.py"]