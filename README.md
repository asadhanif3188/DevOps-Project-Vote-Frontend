# Vote App Frontend 

This is a frontend app, part of [Example Voting App](https://github.com/dockersamples/example-voting-app.git).  

## Steps to Run

To build and run this app as a container, following steps need to be performed in a Dockerfile: 

  * use `python:alpine3.17` container base image
  * map/expose `container port 80`
  * copy over the source code
  * run `pip install -r requirements.txt` to install dependencies
  * launch the app with `gunicorn app:app -b 0.0.0.0:80` command