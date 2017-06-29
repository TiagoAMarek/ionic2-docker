### Build da container
```
sudo docker build -t ionic2-docker --force-rm .
```
### Criando novo projeto
```
sudo docker run -it -v $(pwd):/usr/src/app ionic2-docker ionic start myApp tabs
```
