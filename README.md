# Lab12

## Skład projektu
- **Nginx** - serwer internetowy
- **PHP** - przetwarzanie skryptów serwerowych
- **MySQL** - baza danych
- **phpMyAdmin** - interfejs webowy do zarządzania bazą danych MySQL

## Pliki projektu
- `docker-compose.yml` - konfiguracja wszystkich usług
- `index.php` - przykład skryptu PHP, który łączy się z MySQL
- `default.conf` - konfiguracja Nginxa
- `Dockerfile` - konfiguracja obrazu PHP z potrzebnymi rozszerzeniami
- `mysql_root_password.txt` i `mysql_user_password.txt` - Pliki przechowujące sekrety (nie są uwzględnione w repozytorium).

<img width="1205" alt="image" src="https://github.com/SlaneDRV/DockerLab12/assets/125742851/2d2c08a9-d6ae-44fc-865a-c060422ca68f">



## Uruchamianie projektu
```bash
docker-compose up -d --build
```

## Sprawdzanie działania
```bash
docker-compose ps
```
<img width="973" alt="image" src="https://github.com/SlaneDRV/DockerLab12/assets/125742851/79e9f446-6060-4d3e-b232-7226c8e377dd">

## Nginx: 
http://localhost:4001

<img width="529" alt="image" src="https://github.com/SlaneDRV/DockerLab11/assets/125742851/82865295-fe48-4d2f-8fd7-13cbd7195a60">


Strona startowa Nginx z wynikiem połączenia z MySQL.

## phpMyAdmin: 
http://localhost:6001

<img width="1440" alt="image" src="https://github.com/SlaneDRV/DockerLab12/assets/125742851/53687eb4-28f7-46ce-bb63-f9af763de137">


Interfejs phpMyAdmin do zarządzania bazą danych.

## Zakończenie pracy
```bash
docker-compose down
```
