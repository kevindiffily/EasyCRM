FROM python:3.10

ARG PYTHON_ENV=my_env

ENV PYTHON_ENV=$PYTHON_ENV

RUN mkdir requirements

COPY requirements.txt set_python_env.sh /requirements/

RUN apt update && apt install nano && apt autoremove --purge -y

RUN bash ./requirements/set_python_env.sh $PYTHON_ENV
