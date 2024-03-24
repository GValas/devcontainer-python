# python image
FROM python:3.12
RUN apt update  

# localdir
WORKDIR /app
 
# pip dependencies
RUN pip install --upgrade pip
COPY requirements.txt /app
RUN pip install -r requirements.txt

# copy the scripts to the folder
COPY . /app

# start the server
# CMD ["uvicorn", "main:app", "--host", "0.0.0.0", "--port", "80"]