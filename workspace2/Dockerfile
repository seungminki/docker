# Dockerfile

FROM python:3.7-alpine
WORKDIR /code
RUN python -m pip install --upgrade pip
COPY requirements.txt requirements.txt
RUN pip install -r requirements.txt
EXPOSE 8888
ENTRYPOINT["jupyter"]
COPY . .
CMD ["notebook", "--ip", "0.0.0.0", "--port", "8888", "--allow-root", "--NotebookApp.token='password'"]
