FROM python:3.7

EXPOSE 8888

RUN mkdir -p /usr/src/app
WORKDIR /usr/src/app

COPY requirements.txt /usr/src/app/
RUN pip install --index-url 'https://:2018-09-16T19:22:58.819187Z@time-machines-pypi.sealsecurity.io/' --no-cache-dir -r requirements.txt

COPY . .

ENTRYPOINT ["python3", "blog.py"]
