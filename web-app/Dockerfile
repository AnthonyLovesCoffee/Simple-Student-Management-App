FROM python:3.9-slim

# set a working directory and copy source code to container
WORKDIR /app
COPY . /app

# install dependencies and expoae the port 5000
RUN pip install --no-cache-dir -r requirements.txt
EXPOSE 5000

CMD ["python", "app.py"]
