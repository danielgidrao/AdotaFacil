#usando imagem base do python 3.11 slim
FROM python:3.11-slim

WORKDIR /app

# 1. Copia e instala as dependências (COPY source destino)
COPY requirements.txt requirements.txt
RUN pip install --no-cache-dir -r requirements.txt

# 2. Copia o código do crawler
COPY crawler.py crawler.py

# 3. Executa o crawler
CMD ["python", "crawler.py"]