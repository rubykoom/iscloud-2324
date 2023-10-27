FROM python:3.8-slim-buster

WORKDIR /app

COPY app.py /app
COPY requirements.txt requirements.txt

RUN pip install -r requirements.txt

EXPOSE 5000

ENV MYSQL_ROOT_PASSWORD=p@ssw0rd1

CMD [ "python3" ,"-m" , "flask", "run", "--host=0.0.0.0"]