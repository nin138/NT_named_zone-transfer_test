# DNS zone transfer TEST
# Requirement
- Docker
- Docker Compose
# Usage
1. docker-compose up -d --build
1. docker-compose exec slave bash
1. ls /var/named/slaves (何もない)
1. systemctl start named
1. ls /var/named/slaves (zone fileがある)