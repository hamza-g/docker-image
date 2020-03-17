
FROM debian:9.0
RUN echo "Installation d'apache"
RUN echo "image crée par Hamza"

# Installation  Apache
RUN apt-get update && \
apt-get install -y apache2 && \
apt-get clean

ENV APACHE_LOG_DIR /var/log/apache2

# Utilisation du port 80
EXPOSE 80

# Démarrer Apache
ENTRYPOINT ["/usr/sbin/apache2ctl", "-D", "FOREGROUND"]