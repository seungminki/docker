# Dockerfile

FROM python:3.8
WORKDIR /code
RUN python -m pip install --upgrade pip
COPY requirements.txt requirements.txt
RUN pip install -r requirements.txt
EXPOSE 8888
COPY . /code
ENTRYPOINT ["jupyter"]
CMD ["notebook", "--ip", "0.0.0.0", "--port", "8888", "--allow-root", "--NotebookApp.token='password'"]
