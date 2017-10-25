FROM library/python:3.5-jessie

COPY python/ /opt/python
RUN pip install -r /opt/python/requirements.txt

COPY app/ /opt/app/

EXPOSE 8000

WORKDIR /opt/app/
CMD ["gunicorn", "-b", ":8000", "app:app"]