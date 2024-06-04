FROM python:3-slim

# Set the working directory in the image
WORKDIR /app

# Copy the files from the host file system to the image file system
COPY requirements.txt /app/
COPY devops /app/devops/

# Install the necessary packages
RUN pip install -r --no-cache-dir requirements.txt

ENTRYPOINT ["python3"]

# Run a command to start the application
CMD ["devops/manage.py", "runserver", "0.0.0.0:8000"]
