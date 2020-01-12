FROM python:3.7-slim

RUN python -m pip install --upgrade pip
WORKDIR /app
COPY requirements.txt requirements.txt
RUN python -m pip install -r requirements.txt
COPY .  .
EXPOSE 8000
CMD  sh -c  "python  manage.py runserver  0.0.0.0:8000"
#CMD /usr/local/bin/gunicorn TodoProject.wsgi.application -w 2 -b :8000
