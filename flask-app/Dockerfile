#Use Python Image
FROM python:3.6.8

# Install apt dependencies
RUN apt update -y && apt install python3-pip 

# Copy contents into image
COPY . .

# run pip dependencies
RUN pip3 install -r requirements.txt

# Expose correct port
EXPOSE 5000

# Create an entrypoint
ENTRYPOINT [ "python3", "app.py"]

