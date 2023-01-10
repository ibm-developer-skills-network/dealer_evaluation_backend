FROM python:3.8-slim-buster


WORKDIR /python-docker

COPY requirements.txt requirements.txt
COPY products.json products.json
RUN pip3 install Flask
RUN pip3 install flask_cors

COPY . .

CMD [ "python3", "-m" , "flask", "run", "--host=0.0.0.0"]