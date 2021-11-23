FROM python:3.9

FROM ubuntu:latest

RUN apt-get update -y

# RUN apt-get install -y python3-pip python3-dev build-essential





# copy all the files to the container
COPY . .

# set a directory for the app
WORKDIR /usr/src/app


# install dependencies
RUN apt-get install -y python3-pip python3-dev build-essential
# RUN pip3 install  requirements.txt

RUN pip3 install Flask

RUN pip3 install sklearn

RUN pip3 install scikit-learn



ENTRYPOINT [“python3”]

# tell the port number the container should expose
EXPOSE 5000

# run the command
CMD ["python", "app.py"]
