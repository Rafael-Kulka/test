
# Paytrack API 

Projeto com a API para a integração do Paytrack com o SAP Business One.


# Instalação

Para fazer a instalação da API no servidor de integração, é nescessário configurar as seguintes variaveis de ambiente:

## Variáveis de ambiente

### Service layer: 

- `GOLIVE_SL_USERNAME`: Esta variável deve conter o nome de usuário para acessar a Service Layer.
- `GOLIVE_SL_PASSWORD`: Esta variável deve conter a senha do usuário para acessar a Service Layer.
- `GOLIVE_SL_ENDPOINT`: Esta variável deve conter a URL para acessar a Service Layer no seguinte padrão: https://host:50000/b1s/v1 (incluindo /v1).

### Banco de dados:

- `GOLIVE_DATABASE_TYPE`: Esta variável deve conter o tipo de banco de dados. Valor "HANA" se for hana ou "SQLSERVER" se for SQL Server 2019.

Somente se o ambiente for hana, deve configurar as seguintes variaveis:
- `GOLIVE_HANA_SERVER`: IP do servidor hana.
- `GOLIVE_HANA_USERNAME`: Usuário do banco de dados.
- `GOLIVE_HANA_PASSWORD`: Senha do banco de dados.

Se o ambiente for SQL Server 2019, deve configurar as seguintes variaveis:
- `GOLIVE_SQLSERVER_SERVER`: IP do servidor SQL Server 2019.
- `GOLIVE_SQLSERVER_USERNAME`: Usuário do banco de dados.
- `GOLIVE_SQLSERVER_PASSWORD`: Senha do banco de dados.

## Criação de campos

Após a configuração das variaveis de ambiente, é nescessário criar os campos e tabelas de usuário no SAP Business One seguindo os passos abaixo:

1. Fazer o [download](https://drive.google.com/file/d/1asKU1KXiMNDfY4kK6zyqNlRcJQBqbO3E/view?usp=sharing) do executável.
2. Abrir o SAP Business One, e fazer login na base em que deseja criar os campos.
3. Iniciar o programa CreateFieldAndTable.exe

`* É nescessário um usuário com licença para fazer a criação dos campos.`

`* Após a criação dos campos, fechar o programa CreateFieldAndTable.exe pelo gerenciador de tarefas.`


## Instação da API no IIS.

[Link de referencia de como instalar API no IIS](https://learn.microsoft.com/pt-br/aspnet/core/tutorials/publish-to-iis?view=aspnetcore-9.0&tabs=visual-studio)


