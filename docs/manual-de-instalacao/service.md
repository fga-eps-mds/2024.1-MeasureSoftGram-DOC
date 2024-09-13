# Service

Configura as variáveis de ambiente do repositório. Existe um env-vars-example no projeto, é possível pegar o conteúdo dessa pasta e mover para uma pasta env-vars. Ou você pode criar manualmente a pasta `env-vars` e criar os seguintes arquivos dentro dela: `.service.env` e `.postgres.env`

Na `.postgres.env`:

```bash
POSTGRES_HOST=db
POSTGRES_DB=postgres
POSTGRES_USER=postgres
POSTGRES_PORT=5432
POSTGRES_PASSWORD=postgres
```

Na `.service.env`:

```bash
DEBUG=TRUE
CREATE_FAKE_DATA=TRUE

LOGIN_REDIRECT_URL=http://127.0.0.1:3000/
GITHUB_CLIENT_ID=CLIENT_ID
GITHUB_SECRET=GITHUB_SECRET
SECRET_KEY=django-insecure-9(nkl$g75ia=@q3p*s83rc9y=q5=!q@kr8+s3*xc-t441#jmg%
AMBIENT_TEST_OR_DEV=TRUE
```

É importante salientar que a integração da autenticação do github, assim como a importação de repositórios, só pode ser feita em produção.

Utilize o docker para rodar:

```bash
docker-compose up
```
