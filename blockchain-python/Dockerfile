FROM python:3.6-alpine

WORKDIR /app

# Install dependencies.
ADD requirements.txt /app
RUN pip install -r requirements.txt

# Add actual source code.
ADD blockchain.py /app

EXPOSE 5000

CMD ["python", "blockchain.py", "--host", "0.0.0.0", "--port", "5000"]
