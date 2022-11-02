FROM python:3.7-slim
WORKDIR /app
COPY . .
RUN pip install --upgrade pip
RUN pip install -r /app/api_yamdb/requirements.txt --no-cache-dir
#CMD ["gunicorn", "api_yamdb.wsgi:application", "--bind", "0:8000", "--chdir", "/app/api_yamdb"]
RUN ls
CMD ["python", "/app/api_yamdb/manage.py", "runserver", "0.0.0.0:8000"]