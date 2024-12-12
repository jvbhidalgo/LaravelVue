# Classifrutas Starter Project

Bem-vindo ao **Classifrutas Starter Project**, uma estrutura inicial para projetos utilizando **Laravel**, **Vue.js**, **PostgreSQL** e **Nginx**, totalmente configurada com **Docker**.

---

## 📦 Estrutura do Projeto

```plaintext
projeto/
├── etc/                    # Configurações de serviços
│   ├── nginx/              # Configurações do Nginx
│   ├── php/                # Configuração do PHP
│   └── node/               # Configuração do Node.js
├── web/                    # Código-fonte
│   ├── classifrutas.com.br/
│   │   ├── laravel/        # Backend em Laravel
│   │   └── vue/            # Frontend em Vue.js
├── docker-compose.yml      # Configuração do Docker
└── README.md               # Documentação
```

---

## 🚀 Tecnologias Utilizadas

- **Backend:** Laravel
- **Frontend:** Vue.js
- **Banco de Dados:** PostgreSQL
- **Servidor Web:** Nginx
- **Gerenciamento de Contêineres:** Docker Compose

---

## ⚙️ Configuração Inicial

### **Pré-requisitos**
Certifique-se de ter instalado:
- Docker
- Docker Compose

### **Instalação**

1. Clone o repositório:
   ```bash
   git clone https://github.com/seuusuario/classifrutas-starter.git
   cd classifrutas-starter
   ```

2. Configure suas variáveis de ambiente no arquivo `.env` (exemplo de um `.env` padrão):
   ```dotenv
   APP_ENV=local
   APP_DEBUG=true
   DB_CONNECTION=pgsql
   DB_HOST=db
   DB_PORT=5432
   DB_DATABASE=classifrutas_db
   DB_USERNAME=postgres
   DB_PASSWORD=postgres
   ```

3. Inicie o projeto com Docker Compose:
   ```bash
   docker compose up --build
   ```

---

## 🔧 Como Usar

### Acessos Locais
- **Frontend Vue.js:** [http://classifrutas.local:88](http://classifrutas.local:88)
- **API Laravel:** [http://api.classifrutas.local:88](http://api.classifrutas.local:88)

### Comandos Úteis

```bash
# Subir os contêineres
docker compose up --build

# Parar os contêineres
docker compose down

# Ver logs dos serviços
docker compose logs nginx
```

---

## 📂 Estrutura de Pastas e Serviços

| Serviço   | Caminho                            | Descrição               |
|-----------|------------------------------------|-------------------------|
| Laravel   | `web/classifrutas.com.br/laravel` | Backend API             |
| Vue.js    | `web/classifrutas.com.br/vue`     | Frontend Web            |
| Nginx     | `etc/nginx`                       | Configurações do Nginx  |
| PHP-FPM   | `etc/php`                         | Configurações do PHP    |
| PostgreSQL| Configuração via Docker Compose   | Banco de Dados          |

---

## 🤝 Contribuição

Contribuições são bem-vindas! Siga estas etapas para colaborar:

1. Faça um fork do repositório.
2. Crie uma nova branch:
   ```bash
   git checkout -b feature/sua-feature
   ```
3. Commit suas alterações:
   ```bash
   git commit -m 'Adiciona nova feature'
   ```
4. Envie suas mudanças para o repositório remoto:
   ```bash
   git push origin feature/sua-feature
   ```
5. Abra um Pull Request.

---

## 📝 Licença

Este projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.
