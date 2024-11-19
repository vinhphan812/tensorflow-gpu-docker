FROM tensorflow/tensorflow:2.14.0-gpu-jupyter


RUN apt-get update
RUN pip install -U pip

WORKDIR /app

COPY ./requirements.txt /app
RUN pip install -r /app/requirements.txt

# RUN tensorboard --logdir=YOUR_LOG_DIR --host=127.0.0.1
# %load_ext tensorboard


ENV PYTHONPATH="${PYTHONPATH}:/app"