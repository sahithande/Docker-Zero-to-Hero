# Choose a Python runtime
FROM python:3-slim
# Set the working directory
WORKDIR /app
# Copy requirements.txt and other necessary files
COPY requirements.txt /app/
COPY devops /app/devops/
# Install all the required packages
RUN pip install -r --no-cache-dir requirements.txt
# Set the entrypoint to python
ENTRYPOINT ["python3"]
# Default command to run the django server
CMD ["devops/manage.py", "runserver", "0.0.0.0:8000"]
