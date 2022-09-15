# PHPMyAdmin

PHPMyAdmin para Docker usando Nginx Proxy + Let's Encrypt.

## Dependências

* Docker Compose;
* Repositório [Nginx Proxy + Let's Encrypt](https://github.com/giovannialo/nginx-proxy-letsencrypt).

#### Observação

É necessário realizar os procedimentos de instalação do repositório acima antes de iniciar o processo de instalação
abaixo.

## Instalação

Siga as etapas abaixo para um correto funcionamento do sistema.

### Variáveis de ambiente

Na pasta raiz crie um arquivo chamado **.env**, copie e cole o bloco de código abaixo e configure as variáveis.

```dotenv
VIRTUAL_HOST=phpmyadmin.local
VIRTUAL_PORT=80
LETSENCRYPT_EMAIL=email@exemplo.com
PMA_ARBITRARY=1
```

### Container

Execute o comando abaixo para criar e iniciar o container.

```docker
docker-compose up -d
```

## Credits

* [Giovanni Alves de Lima Oliveira](https://github.com/giovannialo) (Developer)
