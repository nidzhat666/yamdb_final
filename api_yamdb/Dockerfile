FROM python:3.7-slim
WORKDIR /app
COPY . .
RUN ls api_yamdb
RUN pip3 install --upgrade pip
RUN pip3 install -r api_yamdb/requirements.txt --no-cache-dir
CMD ["gunicorn", "--chdir", "/code/myproject", "api_yamdb.wsgi:application", "--bind", "0:8000"]