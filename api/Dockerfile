FROM python:3.9-slim

# set a working directory and copy source code to container
WORKDIR /app
COPY . /app

# install dependencies and expoae the port 8080
RUN pip install --no-cache-dir -r requirements.txt
EXPOSE 8080

# start FastAPI when the container runs
CMD ["uvicorn", "main:app", "--host", "0.0.0.0", "--port", "8080"]
