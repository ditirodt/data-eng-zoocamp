#Specify the base image for the container
FROM python:3.10

#install packages/libraries
#Execute these commands to build and configure the image
RUN apt-get install wget
RUN pip install pandas sqlalchemy psycopg2 pyarrow


#sets the working directory for the container
WORKDIR /app

#copy files/directories from the host machine to the container
COPY ingest_data.py ingest_data.py


#command to ran when the container starts
ENTRYPOINT [ "python","ingest_data.py" ]