# Track map

## Objetivo

Mapa vetorial para:

- app: ponto do carro local ao vivo;
- site: animação decorativa, sem relação com telemetria real;
- replay futuro: múltiplos carros de diferentes usuários.

## Formato

- SVG transparente, sem fundo.
- Linha branca, grossa, cantos arredondados.
- Start/finish quadriculado.
- Setores opcionais em laranja.

## Geração

1. Capturar 3-5 voltas limpas com posição.
2. Filtrar outlap/pit/outliers.
3. Alinhar pelo start/finish.
4. Resample por distância.
5. Mediana + suavização.
6. Fechar loop.
7. Validar comprimento.
8. Gerar JSON + SVG.

## Limitações

- As 15 voltas antigas não têm posição; não servem para o mapa.
- Corrida com tráfego adiciona ruído; hotlap é melhor para o mapa base.
- GT7 não expõe outros carros; AC pode, no futuro.

## Licença

Traçado derivado da própria telemetria. Não copiar arte oficial de mapas.
