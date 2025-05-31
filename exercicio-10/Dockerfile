
FROM python:3.11-slim
WORKDIR /app
COPY app.py .
RUN adduser --disabled-password --gecos '' meuuser
USER meuuser
CMD ["python", "app.py"]
