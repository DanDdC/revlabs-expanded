# RevLabs — Identidade visual

Extraído do protótipo v1. Serve como referência para o novo site.

## Conceito

Laboratório de performance de motorsport: escuro, técnico, glass, laranja de
destaque, dados e telemetria.

## Cores

```css
--bg-dark: #050608;
--orange: #ff4d00;
--orange-soft: rgba(255, 77, 0, 0.18);
--orange-border: rgba(255, 77, 0, 0.45);
--glass: rgba(8, 10, 14, 0.68);
--glass-strong: rgba(8, 10, 14, 0.86);
--glass-border: rgba(255, 255, 255, 0.09);
--text-main: #ffffff;
--text-muted: #9ba0aa;
--text-soft: #c7cad1;
--shadow-orange: 0 0 28px rgba(255, 77, 0, 0.22);
--card-gradient: linear-gradient(145deg, rgba(14, 16, 22, 0.8), rgba(6, 8, 12, 0.68));
```

Uso:
- laranja: marca, kicker, foco, setores, estados ativos;
- branco: títulos e dados principais;
- cinza: textos secundários;
- vidro: cards, nav e modais.

## Tipografia

- Fonte: Inter.
- Títulos: peso 800–900, uppercase, letter-spacing.
- Kicker: 0.75rem, peso 900, letter-spacing 3px, laranja.
- Corpo: 0.9–1rem, `--text-soft`.
- Dados numéricos: tabular, sem serifa.

## Layout

- Nav fixa, centralizada, glass, radius 14px.
- Hero em tela cheia com vídeo de fundo.
- Grid de cards com gap generoso.
- Sidebar no dashboard.
- Modais centralizados com backdrop escuro.

## Componentes

### Card
```css
background: var(--card-gradient);
border: 1px solid var(--glass-border);
border-radius: 16px;
backdrop-filter: blur(22px);
box-shadow: 0 24px 80px rgba(0, 0, 0, 0.36);
```

Hover: borda laranja, leve lift.

### Botão primário
```css
background: linear-gradient(135deg, #ff4d00, #ff7a18);
border-radius: 10px;
color: #fff;
font-weight: 800;
letter-spacing: 1px;
text-transform: uppercase;
box-shadow: var(--shadow-orange);
```

### Botão secundário
Transparente, borda laranja no hover.

### Inputs
Radius 10px, fundo escuro, foco com glow laranja.

### Tabelas
Cabeçalho uppercase, linhas com borda sutil, números tabulares.

## Vídeo de fundo

- Vídeo stock licenciado, carro em pista.
- `filter: blur(7px) brightness(0.58) saturate(1.05)`.
- `transform: scale(1.035)`.
- Overlay:
  - radial laranja no canto superior;
  - gradiente horizontal escuro;
  - gradiente vertical escuro.
- Poster fallback obrigatório.
- `prefers-reduced-motion`: pausar/esconder.

## Track map

- SVG transparente.
- Linha branca, grossa, cantos arredondados.
- Start/finish quadriculado.
- Setores em laranja (opcional).
- Pontos coloridos para carros.
- No site: animação decorativa.
- No app: posição real do carro local.

## Movimento

- Hover: 150–250ms.
- Modais: fade/scale suave.
- Scrollbar laranja.
- Respeitar `prefers-reduced-motion`.

## Acessibilidade

- Contraste mínimo AA.
- Foco visível.
- Não depender só de cor para status.
- Textos alternativos em imagens.
- Vídeo sem áudio e com controle de movimento.

## Assets

- Não portar assets de GT7 para o repositório público.
- Usar stock licenciado, originais ou placeholders.
- Registrar tudo em `assets-manifest.md`.
