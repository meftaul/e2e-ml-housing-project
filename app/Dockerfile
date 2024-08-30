# Install python
FROM python:3.11-slim

# Copy your code
WORKDIR /app
ADD . /app

# Install dependency
RUN pip install -r requirements.txt

EXPOSE 8501

# Run the appliction
ENTRYPOINT ["streamlit", "run", "app.py", "--server.port=8501", "--server.address=0.0.0.0"]