# 1 
FROM python:3.8

# 2
RUN pip install Pillow Flask tensorflow>=2.0.0

# 3
COPY src/ /app
WORKDIR /app

# 4
ENV PORT 8080

# 5
CMD exec gunicorn --bind :$PORT --workers 1 --threads 8 app:app