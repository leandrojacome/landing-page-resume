# Leandro Jácome — Portfólio

Landing page estática, responsiva e acessível para `leandro.srv.br`.

## Executar

```sh
docker build -t landing-page-resume:latest .
docker run --rm -p 8080:80 landing-page-resume:latest
```

O healthcheck está disponível em `/healthz`.

## Swarm

A stack `leandro-resume-preview` usa rede overlay isolada, publica somente a porta
`8086` e fixa o serviço no nó `srv1798039`. O preview esperado é
`http://177.7.34.164.sslip.io:8086`.
