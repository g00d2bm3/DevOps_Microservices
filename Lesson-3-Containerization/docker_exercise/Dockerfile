FROM python:3.8

# Working Directory
WORKDIR /app

# Copy source code to working directory
COPY . /app

# Install packages from requirements.txt
# hadolint ignore=DL3013
RUN pip install --upgrade pip &&\
    pip install -r requirements.txt

# Expose port 5000
EXPOSE 5000

# Run app.py at container launch
CMD ["python", "app.py"]