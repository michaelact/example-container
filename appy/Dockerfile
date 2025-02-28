# This file is used by `docker build`

FROM ubuntu:22.04

RUN apt-get update && apt-get install -y python3.12 python3-pip

COPY requirements.txt .

RUN pip3 install --no-cache-dir -r requirements.txt

COPY . .

EXPOSE 5001

CMD ["python3", "app.py"]
