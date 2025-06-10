
# LEMP + phpMyAdmin - docker-compose

## Uruchomienie

```
docker-compose up -d
```

## Sprawdzenie działania

### 1. Nginx + PHP

Otwórz przeglądarkę i przejdź pod adres:  
[http://localhost:4001](http://localhost:4001)

Wyświetli się strona `phpinfo()`.

### 2. phpMyAdmin

Przejdź pod adres:  
[http://localhost:6001](http://localhost:6001)

Zaloguj się danymi:
- **host**: `mysql`
- **user**: `root`
- **password**: `rootpass`

Po zalogowaniu utwórz bazę danych `testowa`.

## Użyte polecenia

```
docker-compose up -d
docker ps
docker exec -it <mysql-container-id> mysql -u root -p
# następnie w mysql:
SHOW DATABASES;
```

## Dowód działania

- Strona `index.php` się wyświetla ✅
- phpMyAdmin działa i pozwala utworzyć bazę ✅
- Testowa baza danych została utworzona ✅
