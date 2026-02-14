# VeiculosAPI - Sistema de Gerenciamento (Minimal APIs)

[![.NET 10](https://img.shields.io/badge/.NET-10.0-512bd4)](https://dotnet.microsoft.com/download)
[![MySQL](https://img.shields.io/badge/MySQL-005C84?logo=mysql&logoColor=white)](https://www.mysql.com/)
[![JWT](https://img.shields.io/badge/JWT-black?style=flat&logo=json-web-tokens)](https://jwt.io/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

### Descrição do Projeto

Esta é uma API REST de alta performance desenvolvida com **ASP.NET Core Minimal APIs** no ecossistema **.NET 10**. O projeto foi construído para oferecer um sistema de gerenciamento de veículos e administradores, focando em simplicidade de código e robustez na execução.

O sistema conta com autenticação segura, persistência de dados em MySQL e uma arquitetura limpa, ideal para aplicações escaláveis.

---

### Funcionalidades

- **Segurança & Autenticação**: Implementação de JWT (JSON Web Tokens) com suporte a perfis de acesso (**Admin** e **Editor**).
- **Gestão de Veículos**: CRUD completo (Create, Read, Update, Delete) com validações de domínio.
- **Controle de Administradores**: Gerenciamento de usuários com permissões administrativas.
- **Arquitetura Moderna**: Uso de Minimal APIs para redução de boilerplate e ganho de performance.
- **Documentação Automática**: Integração total com Swagger/OpenAPI para testes em tempo real.
- **Testes Automatizados**: Suíte de testes unitários e de integração com xUnit.
- **Seed de Dados**: Sistema de inicialização automática de um administrador padrão para o primeiro acesso.

---

### Tecnologias Utilizadas

- **Framework:** .NET 10.0
- **ORM:** Entity Framework Core 10.0
- **Database:** MySQL (via Pomelo Entity Framework Core 10.0)
- **Auth:** Microsoft AspNetCore Authentication JwtBearer
- **Documentação:** Swashbuckle / OpenAPI
- **Testes:** xUnit & FluentAssertions

---

### Como Executar o Projeto

1. **Clone o repositório:**
   ```bash
   git clone [https://github.com/Souldrow/VeiculosAPI.git](https://github.com/HickSouldrow/VeiculosAPI.git)
   cd VeiculosAPI/api
   ```
2. **Configuração do Banco de Dados:**

- No arquivo appsettings.json, insira sua connection string:

```bash
"ConnectionStrings": {
  "MySql": "Server=localhost;Database=veiculos_db;Uid=root;Pwd=SUA_SENHA;"}
```

3. **Migrations e Build:**

```bash
dotnet restore
dotnet ef database update
```

4. **Execução:**

```bash
dotnet run
dotnet watch
```
