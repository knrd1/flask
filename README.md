# flask
flask
http://flask.pocoo.org/docs/0.12/quickstart/


# Notes for nginx:

        location / {
        include proxy_params;
        proxy_pass http://127.0.0.1:8000;
        }

