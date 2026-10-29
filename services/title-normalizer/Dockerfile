FROM python:3.12-slim
WORKDIR /tasks-api
COPY requirements.txt requirements.txt
RUN pip install -r requirements.txt

COPY . .
EXPOSE 5000



CMD ["python", "-m", "flask", "--app", "app:create_app", "run", "--host=0.0.0.0", "--port=5001"]