# Step 1: Start with a base image
FROM ubuntu:latest

# Step 2: set /app as working folder
WORKDIR /app

# Step 3: install python and pip3
RUN apt-get update && apt-get upgrade -y && \
apt-get install -y python3 python3-pip

# Step 4: remove the EXTERNALLY-MANAGED restriction
RUN rm /usr/lib/python*/EXTERNALLY-MANAGED

# Step 5: install Flask with pip3
RUN pip3 install flask

# Step 6: copy the api.py file into the image
COPY api.py /app/

# Step 7: epose port 5252
EXPOSE 5252

# Step 8: run Flask
CMD ["python3", "api.py"]