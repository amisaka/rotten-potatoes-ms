FROM python:3.8-slim-buster
WORKDIR /app
# Copiar o arquivo de requirements para o python
COPY requirements.txt .
RUN python -m pip install -r requirements.txt
# Copiando os arquivos
COPY . /app
# Expor a port 5000
EXPOSE 5000
# Executar o comando
#CMD ["gunicorn", "--workers=3","--bind", "0.0.0.0:5000", "app:app"]
CMD ["python", "app.py"]
