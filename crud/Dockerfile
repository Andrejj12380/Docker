FROM python:3.10

COPY ./requirements.txt /src/requirements.txt

RUN pip3 install -r /src/requirements.txt

COPY . /src

EXPOSE 6060

WORKDIR /src

RUN python manage.py migrate

CMD ["python", "manage.py", "runserver", "0.0.0.0:6060"]