# Imagem base do Python 3.11
FROM python:3.11

# Diretório de trabalho dentro do container
WORKDIR /app

# Copiar ficheiro de dependências
COPY requirements.txt .

# Instalar dependências Python
RUN pip install --no-cache-dir -r requirements.txt

# Copiar todo o código da aplicação
COPY . .

# Comando para iniciar a API (usando Uvicorn)
CMD ["uvicorn", "app:app", "--host", "0.0.0.0", "--port", "8000"]
