FROM python:3.12

WORKDIR webapp/

COPY requirements.txt .

RUN pip install --no-cache-dir -r requirements.txt

COPY . . 

CMD ["gunicorn", "-w", "4", "-b", "0.0.0.0:8080", "app:app"]
