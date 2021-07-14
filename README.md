# TIO-PATINHAS-NOTIFICACAO-API

## Quais são as tecnologias utilizadas?

- Golang

## O que é este projeto?

- API responsável por gerenciar notificações

### Clone do projeto

```sh
git clone https://gitlab.luizalabs.com/luizalabs/tio-patinhas-notificacao-api.git
```

## Instalação

```sh
go get
```

## Variáveis de ambiente

- "DBUSER": Nome de usuário do banco;
- "DBPASSWORD": Senha do usuário no banco;
- "DBNAME": Nome do banco de dados;
- "DBHOST": IP ou DNS do banco de dados;
- "DBPORT": Porta do banco de dados;
- "TZ": Time Zone no qual a aplicação irá rodar


### Start

Para execução do projeto rodar o comando abaixo

```sh
go run main.go
```

### Tests

Para execução dos testes automatizados executar o comando abaixo no terminal dentro da pasta da aplicação

```sh
go test -v -cover ./...
```

Para gerar a interface mostrando todos os arquivos e as linhas "Covered", "Not Covered" e "Not Tracked":

```sh
go test ./... -coverprofile fmtcoverage.html fmt
go test ./... -coverprofile cover.out
go tool cover -html=cover.out -o cover.html
open 'cover.html' file
```