FROM python:3.9.1

COPY requirements.txt requirements.txt
RUN apt install wget
RUN pip install pandas sqlalchemy psycopg2
# RUN pip install -r requirements.txt

WORKDIR /app
COPY ingest_data.py ingest_data.py

ENTRYPOINT [ "python", "ingest_data.py" ]