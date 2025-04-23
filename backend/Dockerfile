# Use the official Python image from the Docker Hub
FROM python:3

# Set the working directory in the container
WORKDIR /usr/src/app

# Copy the application source code into the container
COPY . .

# Install the dependencies
RUN pip install --no-cache-dir --upgrade -r ./requirements.txt

EXPOSE 3001

# Command to run the FastAPI application
CMD ["python", "./src/server.py"]