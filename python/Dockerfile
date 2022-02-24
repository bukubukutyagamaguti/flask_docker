FROM python:3.6

RUN mkdir /var/log/uwsgi
WORKDIR /var/www

COPY requirements.txt ./
RUN pip install --no-cache-dir -r requirements.txt
RUN apt-get update && apt-get install lsof

# CMD ["uwsgi","--ini","/var/www/uwsgi.ini"]
