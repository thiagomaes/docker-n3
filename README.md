# Webservices Docker Stack

Este repositório contém uma stack Docker para configurar um ambiente web completo com:

- **Nginx** como proxy reverso, servindo o WordPress em `/prova`
- **WordPress** como CMS
- **MySQL 5.7** como banco de dados
- **phpMyAdmin** para administração do MySQL via interface web

---

## 🛠 Pré-requisitos

- Docker instalado
- Docker Compose instalado

---

## 🚀 Como usar

1. Clone este repositório:
```bash
git clone https://github.com/seu-usuario/webservices-docker.git
cd webservices-docker
```

2. Inicie os containers:
```bash
docker compose up -d
```

3. Acesse no navegador:
- WordPress: [http://localhost/prova](http://localhost/prova)
- phpMyAdmin: [http://localhost:8080](http://localhost:8080)

---

## ⚙️ Configurações

- MySQL
  - Usuário: `user`
  - Senha: `password`
  - Banco de dados: `wordpress`
- Nginx redireciona `/` para `/prova`
- Os dados do banco são persistidos no volume `mysql_data`

---

## 🛑 Parar os containers

```bash
docker compose down -v
```

---

## ⚠️ Observações

- Certifique-se de que as portas **80**, **3306** e **8080** estejam livres
- A stack pode demorar alguns segundos para ficar totalmente acessível após o `up`

---

## 🤝 Contribuições

Pull requests são bem-vindos! Para mudanças maiores, abra uma issue para discussão prévia.

---

## 👥 Autores

<table>
  <tr>
    <td align="center">
      <a href="https://github.com/thiagomaes">
        <img src="https://github.com/thiagomaes.png" width="100px;" alt="Thiago Maes"/>
        <br />
        <sub><b>Thiago Maes</b></sub>
      </a>
    </td>
    <td align="center">
      <a href="https://github.com/gabrielmassaia">
        <img src="https://github.com/gabrielmassaia.png" width="100px;" alt="Gabriel Massaia"/>
        <br />
        <sub><b>Gabriel Massaia</b></sub>
      </a>
    </td>
    <td align="center">
      <a href="https://github.com/LucasSetterVeiga">
        <img src="https://github.com/LucasSetterVeiga.png" width="100px;" alt="Lucas Setter Veiga"/>
        <br />
        <sub><b>Lucas Setter Veiga</b></sub>
      </a>
    </td>
  </tr>
</table> 

---

## 📄 Licença

Distribuído sob a licença MIT.
