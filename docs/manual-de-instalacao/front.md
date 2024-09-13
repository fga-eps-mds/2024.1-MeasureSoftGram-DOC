# Front

Configure as variáveis de ambiente transferindo o conteúdo do arquivo `.env.example` para o arquivo `.env`:

```bash
SERVICE_URL=http://localhost:8080
NEXT_PUBLIC_API_URL=http://localhost:8080
LOGIN_REDIRECT_URL=http://127.0.0.1:3000
GITHUB_CLIENT_ID=
GITHUB_SECRET=

```

É importante salientar que a integração da autenticação do github, assim como a importação de repositórios, só pode ser feita em produção.

Utilize o docker para rodar:

```bash
docker-compose up
```

Ou rode manualmente:

```bash
yarn

yarn dev
```
