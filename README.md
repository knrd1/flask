# Flask
Application is reading "index.html" from "templates"

# Requirements for python 3.5 + flask 0.12 + gunicorn + virtual env:

        apt-get update
        apt-get install python3-pip python3-dev nginx -y
        pip3 install virtualenv wheel
        mkdir blog
        cd blog
        virtualenv blogenv
        source blogenv/bin/activate
        pip3 install gunicorn flask
        gunicorn www:app
        deactivate

# Notes for nginx:
        location / {
        include proxy_params;
        proxy_pass http://127.0.0.1:8000;
        }

