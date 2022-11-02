FROM python:3.7-slim
WORKDIR /app
COPY . .
RUN pip install --upgrade pip
RUN pip install -r /app/api_yamdb/requirements.txt --no-cache-dir
RUN python /app/api_yamdb/manage.py collectstatic --noinput
CMD ["gunicorn","--bind", "0:8000", "/app/api_yamdb/api_yamdb.wsgi:application"]
#CMD ["python", "/app/api_yamdb/manage.py", "runserver", "0.0.0.0:8000"]
