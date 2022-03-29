# Aula 1 Iniciativa Kubedev
## _Desafio 1_

### Tarefa

Show de bola !!! A galera ficou MUITO animada, mas querem ver algo mais prático. Então agora, você deve pegar o projeto de conversão de temperatura no GitHub e fazer todo o processo pra executar em containers Docker.Segue o link do projeto no GitHub: https://github.com/KubeDev/conversao-temperatura Faça um fork do repositório, monte o processo de execução no Docker e compartilha aqui o seu repositório. *


## Para Rodar a aplicação

### Criando a Imagem localmente

- fazer um clone desse repositório
```sh
git clone git@github.com:wellsud/conversao-temperatura.git
```
- Acessar a pasta com o codigo fonte
```sh
cd /conversao-temperatura/src
```
- criar a imagem a partid do Dockerfile
```sh
docker image build -t nomedaimagem:tag .
```
- criar o container 
```sh
 docker container run -d -p 8080:8080 nomedaimagem:tag
```

### Através de Imagem no Docker Hub

Como um extra coloquei a imagem no dockerhub. Para executar a aplicação diretamente.

```sh
 docker container run -d -p 8080:8080 wellsud/conversao-temperatura:aula1
