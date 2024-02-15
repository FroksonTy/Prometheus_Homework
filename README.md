# Prometheus_Homework
Homework №1 for OTUS

# Этапы
p.s. В качестве тестовой операционной системы была взяла Astra Linux Spectial Edition 1.7.3

1. Создание виртуальной машины и установка ОС
2. Установка Docker + Docker compose
3. Установка и настройка nginx
4. Установка php8.1-fpm, расширение mysqli
5. Установка и настройка mariadb, создание польователя, базы данных
6. Развертывание CMS WordPress **(:8080)**
7. Развертывание prometheus: /etc/prometheus# "**docker run -d -p 9090:9090 --user root -v ./prom_data:/prometheus -v ./prometheus.yml:/etc/prometheus/prometheus.yml --name prom prom/prometheus**"
8. Установка node_exporter и настройка (/etc/systemd/system/node_exporter.service)
9. Установка blackbox и настройка (/lib/systemd/system/blackbox.service).
10. В конфиге prometheus.yml добавил job'ы для prometheus, docker, node_exporter и blackbox (разделил на два job'а согласно документации на гитхабе:
                                                                                                                                                    job blackbox          - добавил таргеты на веб-сайты (в т.ч. сайт WP на порту :8080)
                                                                                                                                                    job blackbox_exporter - порт :9115
![Uploading изображение.png…]()

    
