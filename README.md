# djp-template

A [ddb](https://inetum-orleans.github.io/docker-devbox-ddb) jsonnet package (**djp**).

## Description

[NodeJS](https://nodejs.org/) **djp** package.

## Snippet

- `ddb.yml`

```yaml
cookiecutter:
  templates:
    - template: gh:inetum-orleans/djp-node
      extra_context:
        node_version: "14"
```

- `docker-compose.yml.jsonnet`

```jsonnet
ddb.Compose(
  ddb.with(
    import '.docker/node/djp.libjsonnet'
  )
)
```

## Parameters

| name  | type | description |
| ------------- | ------------- | ------------- |

## Usage

Please check [jsonnet feature](https://inetum-orleans.github.io/docker-devbox-ddb/features/jsonnet/#ddb-jsonnet-packages-djp)
to understand how to include a **djp** package inside a [ddb](https://inetum-orleans.github.io/docker-devbox-ddb) project.

Looking for other [djp packages](https://github.com/inetum-orleans?q=djp-) ? Check github repositories starting with `djp-`.
