FROM python:3.11-slim

COPY . /app
WORKDIR /app

RUN pip install -r requirements.txt

EXPOSE 8000
VOLUME /models

CMD ["uvicorn", "main:app", "--host", "0.0.0.0", "--port", "8000" ]

# docker build . --tag estate_model:1
# docker run -p 8001:8000 -v $(pwd)/../models:/models estate_model:1