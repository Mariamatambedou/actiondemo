# Utiliser une image de base Python
FROM python:3.9-slim

# Définir le répertoire de travail dans le conteneur
WORKDIR /app

# Copier le fichier requirements.txt depuis le répertoire src dans le conteneur
COPY ../src/requirements.txt .

# Installer les dépendances
RUN pip install --no-cache-dir -r requirements.txt

# Copier le reste du code depuis le répertoire src dans le conteneur
COPY ../src .

# Exposer le port sur lequel l'application tournera
EXPOSE 5000

# Spécifier la commande pour démarrer l'application
CMD ["python", "run.py"]
