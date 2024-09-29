FROM ubuntu:latest
LABEL authors="bthnd"

# Gerekli paketleri yükleyin
RUN apt-get update && \
    apt-get install -y mysql-server && \
    apt-get clean && \
    rm -rf /var/lib/apt/lists/*

# MySQL'i başlatmak için uygun yapılandırma
EXPOSE 3306
CMD ["mysqld"]