FROM python:3.12.3
WORKDIR /web-site
COPY . .
RUN pip install flask gunicorn
EXPOSE 8080
CMD ["gunicorn", "-w", "4", "-b", "0.0.0.0:8080", "app:app"]
