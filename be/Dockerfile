# Dockerfile for Backend Service
FROM python:3.12-slim
ENV APP_HOME=/usr/src/app
ENV APP_PORT=5001
WORKDIR $APP_HOME
COPY requirements.txt .
COPY src/main.py .
RUN pip install --no-cache-dir -r requirements.txt
COPY . .
EXPOSE $APP_PORT
CMD ["python", "main.py"]
