# Basis-Image
FROM alpine:latest

# Installiere benötigte Pakete
RUN apk add --no-cache curl bash

# Setze das Arbeitsverzeichnis
WORKDIR /app

# Kopiere das Shell-Skript und die Konfigurationsdatei ins Image
COPY download_files.sh .

# Gib dem Skript Ausführungsrechte
RUN chmod +x download_files.sh

# Definiere den Befehl, der beim Start des Containers ausgeführt wird
CMD ["./download_files.sh"]

