# Étape 1 : Utiliser une image de base Python officielle
FROM python:3.9-slim

# Étape 2 : Définir le répertoire de travail dans le conteneur
WORKDIR /app

# Étape 3 : Copier les fichiers de dépendances dans le conteneur
COPY requirements.txt .

# Étape 4 : Installer les dépendances Python
RUN pip install --no-cache-dir -r requirements.txt

# Étape 5 : Copier le reste du code de l'application dans le conteneur
COPY . .

# Étape 6 : Exposer le port sur lequel l'application va tourner (ex: 5000 pour Flask)
EXPOSE 5000

# Étape 7 : Spécifier la commande pour démarrer l'application
CMD ["python", "app.py"]
