# HDC Events

Projeto desenvolvido em Laravel para gerenciamento de eventos.
A aplicação permite que usuários façam login, criem eventos, visualizem eventos disponíveis, participem de eventos criados por outros usuários e gerenciem seus próprios eventos pelo dashboard.

## Sobre o projeto

O **HDC Events** é um sistema web simples para organização de eventos.
Cada usuário pode se cadastrar, acessar sua conta, criar eventos e acompanhar tanto os eventos que criou quanto os eventos em que está participando.

Este projeto foi desenvolvido com foco em aprendizado de Laravel, autenticação, relacionamento entre tabelas e manipulação de dados com banco MySQL.

## Funcionalidades

* Cadastro de usuários
* Login e autenticação
* Criação de eventos
* Listagem de eventos
* Visualização de detalhes de um evento
* Edição de eventos
* Exclusão de eventos
* Participação em eventos
* Dashboard com:

  * Meus eventos
  * Eventos que estou participando
* Relacionamento entre usuários e eventos
* Upload de imagem para eventos

## Tecnologias utilizadas

* PHP
* Laravel
* Laravel Jetstream
* Livewire
* MySQL
* Blade
* HTML
* CSS
* Bootstrap
* Vite
* Composer
* NPM

## Requisitos

Antes de rodar o projeto, é necessário ter instalado:

* PHP
* Composer
* Node.js
* NPM
* MySQL
* Git

## Como instalar o projeto

Clone o repositório:

```bash
git clone https://github.com/PedroBerardo0410/Laravel_project.git
```

Entre na pasta do projeto:

```bash
cd Laravel_project
```

Instale as dependências do PHP:

```bash
composer install
```

Instale as dependências do Node:

```bash
npm install
```

Crie o arquivo `.env`:

```bash
cp .env.example .env
```

Gere a chave da aplicação:

```bash
php artisan key:generate
```

Configure o banco de dados no arquivo `.env`:

```env
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=hdceventscurso
DB_USERNAME=root
DB_PASSWORD=
```

Depois rode as migrations:

```bash
php artisan migrate
```

Execute o Vite:

```bash
npm run dev
```

Em outro terminal, inicie o servidor Laravel:

```bash
php artisan serve
```

Acesse o projeto no navegador:

```bash
http://127.0.0.1:8000
```

## Estrutura principal

Alguns arquivos importantes do projeto:

```bash
app/Http/Controllers/EventController.php
app/Models/Event.php
app/Models/User.php
resources/views/events/
routes/web.php
database/migrations/
public/img/events/
```

## Banco de dados

O projeto utiliza tabelas para usuários, eventos e participação em eventos.

Principais tabelas:

* `users`
* `events`
* `event_user`
* `sessions`
* `cache`
* `personal_access_tokens`
* `passkeys`

A tabela `event_user` é responsável por relacionar usuários aos eventos em que estão participando.

## Comandos úteis

Rodar migrations:

```bash
php artisan migrate
```

Ver status das migrations:

```bash
php artisan migrate:status
```

Limpar cache do Laravel:

```bash
php artisan optimize:clear
```

Rodar o servidor:

```bash
php artisan serve
```

Rodar o frontend:

```bash
npm run dev
```

## Autor

Desenvolvido por **Pedro Berardo** como projeto de estudo em Laravel.
