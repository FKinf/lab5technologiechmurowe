# Lab5 - Technologie Chmurowe

## Budowanie obrazu
docker build --build-arg VERSION=1.0.0 -t lab5:v1.0 .

## Uruchomienie kontenera
docker run -d -p 8080:80 --name lab5test lab5:v1.0

## Sprawdzenie działania
Przez curl:
curl localhost:8080

Przez przeglądarkę: **http://localhost:8080**

## Sprawdzenie statusu HEALTHCHECK
docker ps --filter name=lab5test

## Autor
Filip Kwietniak - 101609
