# This file is used by `docker build`

FROM ubuntu:20.04

RUN apt-get update && apt-get install -y python3.10 python3-pip

COPY requirements.txt .

RUN pip3 install --no-cache-dir -r requirements.txt

COPY . .

EXPOSE 5000

CMD ["python3", "app.py"]
