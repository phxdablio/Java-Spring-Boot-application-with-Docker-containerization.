# ☕ Java Spring Boot Application with Docker

Aplicação web desenvolvida com Java e Spring Boot, utilizando Maven para gerenciamento de dependências e Docker para execução em ambiente containerizado.

O projeto foi desenvolvido com foco na prática de conceitos de Docker, criação de imagens, execução de containers, mapeamento de portas e containerização de aplicações Java.

## 🚀 Tecnologias

* Java
* Spring Boot
* Maven
* Docker
* Dockerfile
* JSP
* Git
* GitHub

## 📋 Sobre o projeto

Este projeto foi desenvolvido com o objetivo de colocar em prática conceitos relacionados ao desenvolvimento de aplicações Java com Spring Boot e, principalmente, à utilização do Docker para criação e execução de containers.

Durante o desenvolvimento, foram praticados:

* Desenvolvimento de aplicações com Java e Spring Boot
* Utilização de JSP para criação das páginas
* Gerenciamento de dependências com Maven
* Criação e configuração de Dockerfile
* Construção de imagens Docker
* Execução de aplicações em containers
* Mapeamento de portas entre host e container
* Utilização de imagens base para aplicações Java
* Multi-Stage Build
* Versionamento utilizando Git
* Publicação e gerenciamento do projeto no GitHub

## 📦 Pré-requisitos

Para executar o projeto utilizando Docker, é necessário ter instalado:

* Docker
* Git

Para executar a aplicação diretamente pelo Maven, também é necessário:

* Java
* Maven

## 📥 Clonando o projeto

git clone URL_DO_SEU_REPOSITORIO
cd NOME_DO_PROJETO

## 🐳 Executando com Docker

O projeto possui um Dockerfile responsável pela criação da imagem da aplicação.

### 🔨 Criando a imagem

docker build -t spring-boot-docker:1.0 .

O comando utiliza o Dockerfile presente no projeto para construir uma imagem contendo a aplicação e seu ambiente de execução.

### ▶️ Executando o container

docker run -p 8080:8080 spring-boot-docker:1.0

O parâmetro -p 8080:8080 realiza o mapeamento da porta 8080 do computador para a porta 8080 utilizada pela aplicação dentro do container.

Após iniciar o container, acesse:

http://localhost:8080

## 🔍 Verificando os containers

Para visualizar os containers em execução:

docker ps

Para visualizar todos os containers, incluindo os que estão parados:

docker ps -a

Para parar o container:

docker stop NOME_OU_ID_DO_CONTAINER

## 📦 Docker Image x Docker Container

A imagem Docker funciona como um modelo utilizado para criar containers.

O container é uma instância dessa imagem em execução.

Neste projeto, o fluxo de execução é:

Código da aplicação
↓
Maven
↓
Arquivo JAR
↓
Dockerfile
↓
Docker Image
↓
Docker Container
↓
Spring Boot Application

## 🏗️ Dockerfile

O projeto utiliza um Dockerfile para definir como a aplicação será construída e executada dentro de um container.

O Dockerfile é responsável por definir:

* A imagem base utilizada
* O diretório de trabalho
* Os arquivos que serão copiados para a imagem
* O processo de build da aplicação
* A geração do arquivo JAR
* O ambiente utilizado para execução
* O comando responsável por iniciar a aplicação

O projeto utiliza também o conceito de Multi-Stage Build, separando a etapa de construção da aplicação da etapa de execução.

## 🔌 Mapeamento de portas

O projeto utiliza o seguinte mapeamento:

Host: 8080
Container: 8080

Esse mapeamento permite acessar a aplicação que está sendo executada dentro do container através do navegador:

http://localhost:8080

## 📁 Estrutura do projeto

src/
├── main/
│   ├── java/
│   ├── resources/
│   └── webapp/
└── test/

Dockerfile
pom.xml
mvnw
mvnw.cmd
.gitignore
HELP.md

## 🎯 Objetivo

O principal objetivo do projeto é demonstrar conhecimentos práticos em Docker e containerização de aplicações, utilizando uma aplicação Java Spring Boot como ambiente de estudo.

Entre os principais conceitos praticados estão:

* Docker
* Dockerfile
* Docker Images
* Docker Containers
* Multi-Stage Build
* Port Mapping
* Maven
* Spring Boot
* Git
* GitHub

## 📚 Aprendizados

Durante o desenvolvimento, foram adquiridos conhecimentos práticos sobre:

* Criação e configuração de Dockerfiles
* Construção de imagens Docker
* Execução e gerenciamento de containers
* Mapeamento de portas entre host e container
* Utilização de imagens base
* Multi-Stage Builds
* Containerização de aplicações Java
* Execução de aplicações Spring Boot dentro de containers
* Gerenciamento de dependências com Maven
* Versionamento utilizando Git e GitHub

## 📸 Demonstração

Adicione aqui screenshots da aplicação e do container em execução.

Exemplos:

* Aplicação Spring Boot em execução
* Container executando no Docker
* Imagem Docker criada
* Terminal com o container em execução

## 📄 Licença

Este projeto foi desenvolvido para fins de estudo, aprendizado e portfólio.