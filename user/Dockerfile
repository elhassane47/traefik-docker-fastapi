FROM python:3.8

WORKDIR /app


COPY ./requirements.txt .

RUN pip install --upgrade pip

RUN pip3 install -r requirements.txt


COPY . /app


EXPOSE 8001

CMD ["uvicorn", "--host", "0.0.0.0", "--port", "8001", "--reload", "main:app"]

