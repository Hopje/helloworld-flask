# Description

Python helloworld web app using flask.

Reference: https://docs.microsoft.com/en-us/learn/modules/host-a-web-app-with-azure-app-service/

Run:

    pip3 install flask
    flask run
    curl localhost:5000

Containerised:

    docker build --tag helloflask .
    docker run --rm --publish 8000:5000 helloflask
    curl localhost:8000
