# 🌐 Projeto Web – Aula 27  

📘 **Projeto didático de desenvolvimento Full Stack com Docker Compose**  

![Capa do Projeto](https://img.shields.io/badge/Projeto-Web-blue)  
![Status](https://img.shields.io/badge/status-Em%20Desenvolvimento-yellow)  
![Licença](https://img.shields.io/badge/license-MIT-green)  

---

## 📑 Índice
- [📖 Sobre o projeto](#-sobre-o-projeto)  
- [🚧 Status](#-status)  
- [⚙️ Funcionalidades](#️-funcionalidades)  
- [🛠 Tecnologias utilizadas](#-tecnologias-utilizadas)  
- [🏗 Arquitetura](#-arquitetura)  
- [🗄 Banco de Dados](#-banco-de-dados)  
- [🚀 Como executar o projeto](#-como-executar-o-projeto)  
- [📡 Exemplos de uso (API)](#-exemplos-de-uso-api)  
- [🐳 Comandos úteis do Docker](#-comandos-úteis-do-docker)  
- [🤝 Contribuidores](#-contribuidores)  
- [📜 Licença](#-licença)  

---

## 📖 Sobre o projeto
Este projeto organiza em um **monorepo** as camadas de **frontend, backend e banco de dados**, totalmente integradas e orquestradas via **Docker Compose**.  

🎯 Objetivo didático: servir como **laboratório de práticas full-stack**, mostrando como estruturar, configurar e executar um projeto moderno de forma rápida e padronizada.  

Ele demonstra:
- Separação clara entre camadas: **apresentação, lógica de negócio e persistência de dados**;  
- Uso de contêineres para **portabilidade e consistência** do ambiente;  
- Fluxo simples de execução → ideal para iniciantes e revisores de conceitos.  

---

## 🚧 Status
> 🛠 Em desenvolvimento – novas funcionalidades serão adicionadas em breve!  

---

## ⚙️ Funcionalidades
✅ API backend em Node.js (Express)  
✅ Frontend em HTML/JS simples  
✅ Banco de Dados PostgreSQL inicializado via script  
✅ Orquestração com Docker Compose  
🔜 Autenticação de usuários  
🔜 Testes automatizados  

---

## 🛠 Tecnologias utilizadas
- **Frontend** → HTML, CSS, JavaScript  
- **Backend** → Node.js + Express  
- **Banco de Dados** → PostgreSQL  
- **Infra** → Docker & Docker Compose  

---

## 🏗 Arquitetura  

### Estrutura de pastas

# Estrutura de Pastas - Projeto Web Aula 27

📦 projeto_web_aula_27
├── backend/               # API Node.js (Express)
│   ├── server.js          # Código principal da API
│   ├── package.json       # Dependências do backend
│   ├── Dockerfile         # Configuração do container
│   └── .dockerignore      # Arquivos ignorados pelo Docker
├── frontend/              # Camada de apresentação
│   ├── index.html         # Página inicial
│   ├── app.js             # Lógica do frontend
│   └── Dockerfile         # Container do frontend
├── db/                    # Banco de Dados
│   └── init.sql           # Script de inicialização
├── .env                   # Variáveis de ambiente
├── docker-compose.yml     # Orquestração dos serviços
└── README.md              # Documentação do projeto


## 🚀 Como executar o projeto

### Com Docker
1. Clone o repositório:
   ```bash
   git clone https://github.com/ArivaldoFilho/prog_web_docker_test.git
   cd projeto_web_aula_27

2. Configure as variáveis de ambiente no arquivo .env:
    ```bash
    POSTGRES_USER=usuario
    POSTGRES_PASSWORD=senha
    POSTGRES_DB=meubanco

3. Suba os containers:
    ```bash
    docker-compose up --build

4. Acesse os serviços:

    🌍 Frontend → http://localhost:8080

    ⚙️ Backend API → http://localhost:3000

    🗄 Banco de Dados → localhost:5432