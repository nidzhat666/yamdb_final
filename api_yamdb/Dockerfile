FROM python:3.7-slim
WORKDIR /app
COPY . .
ENV PYTHONPATH /app/api_yamdb/
RUN pip install --upgrade pip
RUN pip install -r /app/api_yamdb/requirements.txt --no-cache-dir
CMD ["gunicorn","--bind", "0:8000", "api_yamdb.wsgi:application"]
