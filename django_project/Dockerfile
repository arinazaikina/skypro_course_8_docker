FROM python:3.10-slim

WORKDIR /app

COPY .. /app/

RUN pip install --no-cache-dir -r requirements.txt

CMD ["gunicorn", "config.wsgi:application", "--bind", "0.0.0.0:8000"]
