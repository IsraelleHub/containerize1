# your code goes here ...
# Use the base image with Python
FROM python:3.9-slim

# Set working directory
WORKDIR /app

# Copy application files
COPY ./app/src /app

# Install dependencies
RUN pip install --upgrade pip && \
    pip install -r requirements.txt

# Expose the port the app runs on
EXPOSE 8000

# Start the application with gunicorn
CMD ["gunicorn", "-b", "0.0.0.0:8000", "server:app"]