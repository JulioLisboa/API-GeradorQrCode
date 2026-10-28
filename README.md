# API Gerador de QR Code

API REST para geração de QR Codes e armazenamento dos arquivos em um bucket Amazon S3, utilizando serviços da AWS.

## Objetivo

Este projeto foi desenvolvido para fins de estudo e aprendizado, com o objetivo de aprimorar conhecimentos em desenvolvimento backend, construção de APIs REST, conteinerização e integração com serviços de armazenamento em nuvem.

## Tecnologias utilizadas

- **Java** — linguagem de programação.
- **Spring Boot** — framework para desenvolvimento da API.
- **Maven** — gerenciamento de dependências e build do projeto.
- **Docker** — conteinerização da aplicação.
- **Amazon S3** — armazenamento dos arquivos de QR Code na nuvem.

## Como executar o projeto

### Pré-requisitos

Antes de executar o projeto, você precisará ter instalado:

- [Java](https://www.oracle.com/java/)
- [Docker](https://www.docker.com/)
- Uma conta AWS com as permissões necessárias para acessar o bucket S3.

### 1. Clone o repositório

```bash
git clone https://github.com/JulioLisboa/API-GeradorQrCode.git
```

### 2. Acesse a pasta do projeto

```bash
cd API-GeradorQrCode
```

### 3. Configure as variáveis de ambiente

Crie um arquivo `.env` na raiz do projeto com as variáveis de ambiente necessárias para a aplicação.

Configure as credenciais e os parâmetros de acesso à AWS conforme a implementação do projeto.

> **Importante:** nunca compartilhe credenciais nem envie arquivos `.env` com informações sensíveis para o GitHub.

### 4. Construa a imagem Docker

```bash
docker build -t geradorqrcode .
```

### 5. Execute o container

```bash
docker run --env-file .env -p 8080:8080 geradorqrcode
```

Após a inicialização, a aplicação estará disponível na porta `8080`, desde que não haja erros de configuração.

---

*Este projeto foi desenvolvido exclusivamente para estudo e prática de programação.*