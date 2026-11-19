# RevLabs Expanded

Site, API e engine de análise do RevLabs.

## Objetivo

Receber bundles do `revlabs-telemetry`, validar, armazenar e transformar em:

- catálogo de carros, pistas e peças;
- setup builder;
- lista e comparação de voltas;
- estimativa de tempo de volta;
- análise de hotlap, practice e race.

## Stack planejada

- Django 6 + Django Ninja
- PostgreSQL
- Redis + RQ/Celery
- MinIO local / S3/R2 em produção
- HTMX + Alpine
- engine Python puro

## Escopo do MVP

- catálogo;
- setup builder;
- import de bundle;
- listagem de voltas;
- dashboard hotlap;
- race v0;
- track map decorativo no site.

## Dados legados

`legacy/laps.json` contém apenas metadados das 15 voltas antigas (tempo,
setores, stats). Não há posições/frames; não serve para gerar track map.

## Licença

MIT + Commons Clause. Veja [LICENSE](LICENSE).
