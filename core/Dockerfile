# Usa una imagen base de Python
FROM python:3.12-slim

# Establece el directorio de trabajo en /app
WORKDIR /app

# Copia el archivo de requisitos a la ubicación del contenedor
COPY requirements.txt /app/

# Instala las dependencias
RUN pip install --no-cache-dir -r requirements.txt

# Copia el código de la aplicación a la ubicación del contenedor
COPY . /app/

# Expone el puerto en el que se ejecutará la aplicación Django
EXPOSE 8000

# Comando para ejecutar la aplicación Django
CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]
