## Criação do projeto

#### 1. Build da container
```
sudo docker build -t ionic2-docker --force-rm .
```
#### 2. Criando novo projeto
```
sudo docker run -it -v $(pwd):/usr/src/app ionic2-docker ionic start myApp tabs
```

## Ambiente de desenvolvimento
Antes de começar, dentro do `docker-compose.yml` altere o {NOME_APP} para o nome do diretório do seu app.

#### 1. Build das containers 
```
sudo docker-compose build
```

#### 2. Instalando dependências
```
sudo docker-compose up install_node_modules
```

#### 3. Iniciar o ambiente
```
sudo docker-compose up serve
```