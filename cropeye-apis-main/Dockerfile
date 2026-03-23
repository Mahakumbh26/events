FROM python:3.10-slim
WORKDIR /app
COPY cropeye-apis-main/ .
RUN pip install --no-cache-dir -r requirements.txt

# Default start command, override via START_COMMAND env var in Railway
CMD ["sh", "-c", "${START_COMMAND:-python events.py}"]
