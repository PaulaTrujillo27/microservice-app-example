
FROM python:3.6

# Establecer el directorio de trabajo dentro del contenedor
WORKDIR /app

# Copiar el archivo package.json y package-lock.json (si existe)
COPY . .

RUN pip3 install -r requirements.txt
EXPOSE 6029
ENV REDIS_HOST=redis
ENV REDIS_PORT=6379 
ENV REDIS_CHANNEL=log_channel 
CMD ["python3", "main.py"]