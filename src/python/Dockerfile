FROM python:3.7-alpine
WORKDIR /app
COPY /requirements.txt /app
RUN pip3 install -r requirements.txt
EXPOSE 8080
COPY . /app
ENTRYPOINT [ "python3", "app.py" ]
