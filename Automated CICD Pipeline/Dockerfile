# Base Python image
FROM python:3.9-slim

# Set working directory
WORKDIR /app

# Copy application files
COPY app/ /app

# Install dependencies
RUN pip install --no-cache-dir -r requirements.txt

# Expose the Flask app port
EXPOSE 5000

# Command to run the app
CMD ["python", "app.py"]
