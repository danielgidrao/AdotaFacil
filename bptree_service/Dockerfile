FROM python:3.11-slim

WORKDIR /app

COPY requirements.txt requirements.txt
RUN pip install --no-cache-dir -r requirements.txt

COPY bptree_service.py bptree_service.py

#volume para persistir o arquivo pets.db
VOLUME [ "/data" ]
CMD ["python", "bptree_service.py"]
