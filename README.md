```markdown
# 📦 Warehouse Management System - It Case

Sistema de **gestão de estoque** desenvolvido para a **It Case**, com o objetivo de otimizar o controle de produtos, movimentações de entrada/saída e relatórios de estoque.  
Construído com **Laravel 12** (API RESTful) e **Angular 20** (interface web moderna).

---

## 🚀 Tecnologias Utilizadas

### Backend
- [Laravel 12](https://laravel.com/) - Framework PHP moderno para a API
- [PHP 8.2+](https://www.php.net/) - Linguagem de backend
- [Composer](https://getcomposer.org/) - Gerenciador de dependências
- Banco de dados: **PostgreSQL** (ou outro configurado via `.env`)
- Autenticação JWT (JSON Web Token)

### Frontend
- [Angular 20](https://angular.dev/) - Framework SPA (Single Page Application)
- [TypeScript](https://www.typescriptlang.org/)
- [RxJS](https://rxjs.dev/) para programação reativa
- [Angular Material](https://material.angular.io/) para UI

---

## 📂 Estrutura do Projeto

```

Warehouse-Management-System/
├── client/   # Frontend em Angular 20
└── server/   # Backend em Laravel 12

````

---

## ⚙️ Configuração e Instalação

### 1. Clonar o repositório
```bash
git clone https://github.com/dev-raimundos/Warehouse-Management-System.git
cd Warehouse-Management-System
````

### 2. Configurar o Backend (Laravel 12)

```bash
cd server

# Instalar dependências
composer install

# Copiar o arquivo de ambiente
cp .env.example .env

# Configurar conexão com o banco no arquivo .env
# Exemplo (PostgreSQL):
# DB_CONNECTION=pgsql
# DB_HOST=127.0.0.1
# DB_PORT=5432
# DB_DATABASE=warehouse
# DB_USERNAME=postgres
# DB_PASSWORD=secret

# Gerar a chave da aplicação
php artisan key:generate

# Rodar as migrations
php artisan migrate
```

Rodar o servidor:

```bash
php artisan serve
```

### 3. Configurar o Frontend (Angular 20)

```bash
cd ../client

# Instalar dependências
npm install

# Rodar em ambiente de desenvolvimento
ng serve -o
```

---

## 🌐 Endpoints Principais da API

* `POST /api/login` → autenticação
* `GET /api/products` → listar produtos
* `POST /api/products` → cadastrar novo produto
* `PUT /api/products/{id}` → atualizar produto
* `DELETE /api/products/{id}` → remover produto
* `GET /api/reports/stock` → relatório de estoque

---

## 📊 Funcionalidades

✅ Controle de produtos (cadastro, edição, exclusão)
✅ Movimentação de entrada e saída de estoque
✅ Relatórios gerenciais em tempo real
✅ Autenticação e autorização com JWT
✅ Dashboard interativo no frontend
✅ Integração entre API (Laravel) e SPA (Angular)

---

## 🤝 Contribuição

1. Faça um fork do projeto
2. Crie uma branch para sua feature (`git checkout -b feature/nova-feature`)
3. Commit suas alterações (`git commit -m 'Add nova feature'`)
4. Faça push para a branch (`git push origin feature/nova-feature`)
5. Abra um Pull Request

---

## 📜 Licença

Este projeto foi desenvolvido para **uso interno da It Case**.
Distribuição ou cópia sem autorização prévia não é permitida.

---

## 👨‍💻 Autor

Desenvolvido por **It Case**
Contato: [GitHub - dev-raimundos](https://github.com/dev-raimundos)

```
