# Example Python Dockerfile
FROM python:3.10

WORKDIR /app

# Copy requirements.txt separately for better caching
COPY requirements.txt .

RUN pip install --no-cache-dir -r requirements.txt

# Copy the rest of the application code
COPY app.py .

EXPOSE 5000

CMD ["python", "app.py", "--host", "0.0.0.0", "--port", "5000"]
