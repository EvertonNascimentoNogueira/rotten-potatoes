FROM python:3.8
WORKDIR /app
COPY requirements.txt requirements.txt
RUN pip3 install -r requirements.txt
COPY . .
EXPOSE 5000
CMD [CMD ["gunicorn", "--bind", "0.0.0.0:5000", "-c", "config.py", "app:app"]