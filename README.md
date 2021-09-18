# Trabalho Individual 02 2021.1

## Build

Para executar a aplicação em sua máquina, basta seguir o passo-a-passo a seguir:
Para subir todos os serviços deste projeto:

##### backend

```docker
docker-compose -f backend/docker-compose.yml up -d
```

##### frontend

```docker
docker-compose -f frontend/docker-compose.yml up -d
```

## Testes

Para rodar os testes do frontend:

```docker
docker-compose -f frontend/docker-compose.yml run --entrypoint "npm run test" frontend
```

Para rodar os testes do backend:

```docker
docker-compose -f backend/docker-compose.yml run --entrypoint "npm run unittest" backend
```

## 1. Integração com gitlab

O repositório integrando o serviço com o gitlab é esse [https://gitlab.com/gustavolima00/Workshop-CI-Entrega-02](https://gitlab.com/gustavolima00/Workshop-CI-Entrega-02) nele é feito as pipelines de execução descritas no arquivo **.gitlab-ci.yml**

## 2. Build and Test

- A etapa de build é descrita no arquivo **.gitlab-ci.yml** que realiza o build dos arquivos e os deixa prontos para o deploy.
- A etapa de testes também está descrita no arquivo e realiza testes nas aplicações garantindo a integridade

## Deploy 

TODO 
