
# Use an official Python runtime as a base image
FROM python:3.11

# set the working directory to /app
WORKDIR /app

# Copy the current directory contents into the container at /app
ADD . /app

# Install any needed packages specified in requirements.txt
RUN pip install --no-cache-dir -r requirements

# define the command to start the application using Gunicorn with 4 worker processes
CMD ["gunicorn", "superkart_api:superkart_model", "--workers=4"]
