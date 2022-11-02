FROM python:3.7-slim
WORKDIR /app
COPY . /app
RUN pip install --upgrade pip
RUN pip install -r /app/api_yamdb/requirements.txt --no-cache-dir
#CMD ["gunicorn", "api_yamdb.wsgi:application", "--bind", "0:8000", "--chdir", "/app/api_yamdb"]