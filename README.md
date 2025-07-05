# Webservices Docker Stack

Este repositório contém uma stack Docker para executar um ambiente web completo com:

-   **Nginx** como proxy reverso configurado para servir o WordPress em `/prova`
-   **WordPress** como CMS
-   **MySQL 5.7** como banco de dados
-   **phpMyAdmin** para administração do banco MySQL via interface web

---

## Como usar

### Pré-requisitos

-   Docker instalado na sua máquina
-   Docker Compose instalado

### Passos para rodar

1. Clone este repositório:

```bash
git clone https://github.com/seu-usuario/webservices-docker.git
cd webservices-docker
Inicie os containers:

bash
Copiar
Editar
docker compose up -d
Acesse o WordPress no navegador:

arduino
Copiar
Editar
http://localhost/prova
Para acessar o phpMyAdmin, use:

arduino
Copiar
Editar
http://localhost:8080
Configurações
Banco MySQL está configurado com usuário: user e senha: password

Banco de dados padrão: wordpress

O Nginx redireciona a raiz / para /prova, onde o WordPress está rodando

Parar os containers
bash
Copiar
Editar
docker compose down
Observações
Certifique-se de que as portas 80, 3306 e 8080 não estejam em uso por outros serviços

Os dados do MySQL ficam persistidos no volume Docker mysql_data

Contribuição
Pull requests são bem-vindos! Para mudanças maiores, abra uma issue para discussão prévia.

Autor
Thiago Maes
Gabriel Massaia
Lucas Veiga

Licença
MIT License
```
