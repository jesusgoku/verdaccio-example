# Verdaccio: Private NPM registry

Setting [Verdaccio](https://verdaccio.org/) as a private npm registry.

## Setting

Generate users on [htpasswd generator](https://hostingcanada.org/htpasswd-generator/) and add to `/htpasswd` file.

## Running

```bash
docker-compose up -d
```

## Usage

```bash
# Login on registry
npm login --registry http://0.0.0.0:4873

# Publish a package
npm publish --registry http://0.0.0.0:4873

# Usage package
npm add [some-package] --registry http://0.0.0.0:4873
```

## References

- [Verdaccio Docs](https://verdaccio.org/docs/en/installation)
