# Arquitetura

## Repositórios

- `revlabs-schema`: contrato de dados (MIT)
- `revlabs-telemetry`: app de captura (Tauri + React + Rust)
- `revlabs-expanded`: site/API/engine (Django + HTMX)

## Fluxo

```
GT7 -> RevLabs Telemetry -> bundle .revlabs
                              |
                              v
                     API de import
                              |
                     validação + storage
                              |
                     PostgreSQL + S3
                              |
                     engine de análise
                              |
                        site/API
```

## Princípios

- Servidor é a fonte da verdade.
- Dados brutos são imutáveis; derivados são reprocessáveis.
- Cálculo nunca no cliente.
- Todo dado tem proveniência e versão.
- Nenhum asset de jogo no repositório público.
