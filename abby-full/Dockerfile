FROM ubuntu:latest
LABEL maintainer arjuna.rahman@dsclogistics.com
RUN apt-get update -y && apt-get install -y python-pip
python-dev build-essential
COPY . /app
WORKDIR /app
RUN pip install -r requirements.txt
EXPOSE 5000
ENTRYPOINT ["python"]
CMD ["application.py"]