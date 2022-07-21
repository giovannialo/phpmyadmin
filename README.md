# PHPMyAdmin

PHPMyAdmin para Docker usando Nginx Proxy + Let's Encrypt.

## Dependências

* Repositório [Nginx Proxy + Let's Encrypt](https://github.com/giovannialo/nginx-proxy-letsencrypt).

#### Observação

É necessário realizar os procedimentos de instalação do repositório acima antes de iniciar o processo de instalação abaixo.

## Instalação

Siga as etapas abaixo para um correto funcionamento do sistema.

### Variáveis de ambiente

Faça uma cópia do arquivo **.env.example** para **.env** e configure as variáveis conforme as configurações do seu servidor.

#### Exemplo

```dotenv
PHPMYADMIN_VIRTUAL_HOST=phpmyadmin.meudominio.com.br
PHPMYADMIN_VIRTUAL_PORT=80
PHPMYADMIN_LETSENCRYPT_HOST=phpmyadmin.meudominio.com.br
PHPMYADMIN_LETSENCRYPT_EMAIL=email@exemplo.com
PHPMYADMIN_PMA_ARBITRARY=1
```

### Container

Execute o comando abaixo para criar e iniciar o container.

```docker
docker-compose up -d
```

## Credits

* [Giovanni Alves de Lima Oliveira](https://github.com/giovannialo) (Developer)
