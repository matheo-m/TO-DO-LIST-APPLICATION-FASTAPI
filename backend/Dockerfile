# Use the official Python image from the Docker Hub
FROM python:3

# Set the working directory in the container
WORKDIR /usr/src/app

# Copy the requirements file and install dependencies
COPY requirements.txt .
RUN pip install --no-cache-dir --upgrade -r requirements.txt

# Copy your application code inside the container
COPY src/ ./src

# Expose the port
EXPOSE 3001

# Command to run the FastAPI application
CMD ["python", "./src/server.py"]
