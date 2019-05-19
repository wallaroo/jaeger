FROM python@sha256:d16c1ec3910dbc686fedae33b450e5e492ffd789f63f2917f0c2709d1e6bdb7d

# Temporary fix for https://github.com/jaegertracing/jaeger/issues/1494
RUN pip install urllib3==1.21.1

RUN pip install elasticsearch elasticsearch-curator
COPY esCleaner.py /es-index-cleaner/

ENTRYPOINT ["python3", "/es-index-cleaner/esCleaner.py"]
