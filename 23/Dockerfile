FROM python:3
ADD py-webserver.py /
RUN pip install flask
RUN pip install requests
RUN pip install jsonify
COPY py-webserver.py /opt/
ENTRYPOINT FLASK_APP=/opt/py-webserver.py flask run --host=0.0.0.0 --port=9080