FROM python:3.12.3-slim-bullseye

WORKDIR /app

COPY ./requirements.txt /app/requirements.txt

RUN pip install --no-cache-dir --upgrade -r /app/requirements.txt

# COPY remaininng files
COPY ./ /app/

EXPOSE 80
# COMMAND to launch fastapi app
CMD ["fastapi", "run", "main.py", "--port", "80"]