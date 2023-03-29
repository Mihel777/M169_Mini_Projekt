# Erstellung der Dateien

Zuerst muss im Homeverzeichnis ein Verzeichnis erstellt werden, indem anschliessend das Dockerfile, sowie das PHP File gespeicheert werden kann.

Code:
mkdir apache-php -> Ordner erstellen</br>
cd apache-php -> in den Ordner wechseln</br>
*# Michel Miniprojekt -> auskommentierte Überschrift</br>
FROM php:8-apache -> gibt das Basisimage an</br>
COPY index.php /var/www/html -> Kopiert Dateien aus dem Projektverzeichnis in das Image</br>
RUN apt-get update && apt-get upgrade -y -> führt das angegebene Kommando aus</br>

