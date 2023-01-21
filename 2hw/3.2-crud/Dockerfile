FROM python:3.8
COPY stocks_products/requirements.txt src/requirements.txt
COPY /stocks_products /src
EXPOSE 7447
WORKDIR src
RUN pip3 install --no-cache-dir --upgrade -r /src/requirements.txt && \
    python /src/manage.py migrate
CMD ["python3", "manage.py", "runserver", "0.0.0.0:7447"]