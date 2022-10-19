# load prebuilt images
FROM python:3.8-buster

#make the directories for scripts and apps
RUN mkdir -p /app


# copy the source code to the working directory
COPY requirements.txt app.py /app/

# install packages common to all scripts from "requierements.txt"
WORKDIR /app
RUN pip install --upgrade pip &&\
    pip install --trusted-host pypi.python.org -r requirements.txt 


CMD ["cat", "app.py"]
