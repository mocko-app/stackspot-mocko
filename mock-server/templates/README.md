# {{project_name}}

Este é um servidor de mocks feito usando [Mocko](https://mocko.dev/). Mais informações na documentação em [docs.mocko.dev](https://docs.mocko.dev/).

# Como rodar

## Usando o Mocko CLI

Primeiro instale o Mocko CLI com `npm`:
```bash
npm i -g @mocko/cli
```

Você pode precisar de `sudo` no Linux ou Mac:
```bash
sudo npm i -g @mocko/cli
```

Execute os mocks (exemplo na porta {{port}}) com o seguinte comando:
```bash
mocko --port {{port}} --watch ./mocks
```

## Usando Docker

Builde o servidor usando o Docker:

```bash
docker build -t {{project_name}} ./
```

Rode o container (exemplo na porta {{port}}):
```bash
docker run -p {{port}}:8080 {{project_name}}
```

# Como acessar os mocks

Prontinho! Agora é só usar:
```bash
curl http://localhost:{{port}}/cats/george
```

# Como criar um novo mock

É possível criar mocks dinâmicos, proxiar sua API, persistir dados e muito mais! [Veja a documentação aqui](https://mocko.dev/docs/getting-started/standalone/#using-mocko).
