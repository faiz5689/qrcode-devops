# Pull the base image as python 3.9
FROM python:3.9

# Set the working directory
WORKDIR /usr/src/app

# Copy the requirements file
COPY requirements.txt ./

# Install the dependencies
RUN pip install --no-cache-dir -r requirements.txt

# Copy the source code
COPY . .

# Expose the port and run the server
CMD ["uvicorn", "main:app", "--host", "0.0.0.0", "--port", "80"]