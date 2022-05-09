FROM tiangolo/uvicorn-gunicorn-fastapi:python3.7

WORKDIR /app
COPY . .
RUN /usr/local/bin/python -m pip install --upgrade pip
RUN pip install -r /app/req.txt
EXPOSE 8080

CMD ["uvicorn", "main:app", "--host", "0.0.0.0", "--port", "80", "--reload"]
