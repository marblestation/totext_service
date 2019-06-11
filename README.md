# totext_service
This microservice makes api calls and converts their json responses to text (currently only html).

The /search endpoint accepts a user query, sends it to the api/search endpoint and converts the solr response to html.  Each query reults in a single api call.  This microservices uses Python/Flask/Jinja2 and a template file to create its response.  This HTML page mimics BBB.

It was originally developed for and ads hackathon.

## Run

Execute:

```
python wsgi.py
```

Access: [http://127.0.0.1:4000/](http://127.0.0.1:4000/)
