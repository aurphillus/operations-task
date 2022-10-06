FROM python:3.10-alpine

WORKDIR /app

COPY . .

RUN pip install gunicorn && pip install -r requirements.txt

EXPOSE 3000

CMD ["gunicorn" , "-b", "0.0.0.0:3000", "wsgi"]
