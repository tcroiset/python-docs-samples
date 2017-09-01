FROM gcr.io/google_appengine/python

RUN apt-get update
ADD requirements.txt /app/
RUN pip install -r requirements.txt

ADD . /app
CMD gunicorn -b :$PORT project_name.wsgi
