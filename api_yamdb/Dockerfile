FROM python:3.7-slim
WORKDIR /app
COPY . .
RUN ls api_yamdb
RUN pip3 install --upgrade pip
RUN pip3 install -r api_yamdb/requirements.txt --no-cache-dir
RUN ls /app/
CMD ["python", "manage.py", "runserver", "127.0.0.1:8000"]