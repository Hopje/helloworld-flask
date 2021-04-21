# Description

Python helloworld web app using flask. Edited

Reference: 
    <https://docs.microsoft.com/en-us/learn/modules/host-a-web-app-with-azure-app-service/>
    <https://pythonbasics.org/flask-rest-api/>

Run:

    pip3 install flask
    flask run
    (python3 -m flask run)
    curl localhost:5000

Containerised:

    docker build --tag helloflask .
    docker run --rm --publish 8000:5000 helloflask
    curl localhost:8000/hello

Invoke rest service:

    curl -X PUT -d name=alice -d email=alice@outlook.com localhost:5000
    curl localhost:5000?name=alice
