# Erstellung der Dateien

Zuerst muss im Homeverzeichnis ein Verzeichnis erstellt werden, indem anschliessend das Dockerfile, sowie das PHP File gespeicheert werden kann.

Code:
mkdir apache-php -> Ordner erstellen
cd apache-php -> in den Ordner wechseln
*# Michel Miniprojekt -> auskommentierte Überschrift
FROM php:8-apache -> gibt das Basisimage an
COPY index.php /var/www/html -> Kopiert Dateien aus dem Projektverzeichnis in das Image
RUN apt-get update && apt-get upgrade -y -> führt das angegebene Kommando aus

