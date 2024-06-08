# fiap-gs1

Aplicação Java proposta como global solution do primeiro semestre da matéria de Engenharia Web e Microserviços

## Pré-requisitos

- Java 17+
- Docker
- Acesso a internet
- Acesso ao Docker Hub

# Instalação

#### Clone

```
git clone https://github.com/GabrielPl-1/fiap-gs.git
```

## Execução


#### Docker

* Criação de imagem

```
docker build -t fiap-gs1 .
```

* Executar container

```
docker run -d -p 8080:8080 -e PROFILE=<prd|dev|stg> fiap-gs1
```

* Executar container a partir do Docker Hub


Profile dev
```
docker run -d -p 8080:8080 -e PROFILE=dev gapenna/fiap-gs1
```

Profile stg
```
docker run -d -p 8080:8080 -e PROFILE=stg gapenna/fiap-gs1
```

Profile prd
```
docker run -d -p 8080:8080 -e PROFILE=prd gapenna/fiap-gs1
```
