# Assets manifest

## Inventário do v1

O protótipo tinha aproximadamente:

- 56 imagens (~29,8 MB)
- 1 vídeo (`static/videos/landing/hero-track.mp4`, ~10,9 MB)

## Política

Nada de assets de GT7/PlayStation no repositório público.

| Categoria | Exemplos | Status | Ação |
|---|---|---|---|
| Backgrounds de pista | `img/bg/*.jpg` | Game-derived | Não portar; substituir por stock licenciado |
| Layouts de pista | `img/layout/*.png` | Game-derived/oficial | Não portar; gerar track map da telemetria |
| Carros | `img/cars/*.png` | Game-derived | Não portar; usar placeholders/ilustrações |
| Ícones de peças | `img/mods/*.png` | Game-derived | Não portar; criar ícones próprios |
| Vídeo hero | `videos/landing/hero-track.mp4` | Game-derived | Não portar; usar stock licenciado |
| Avatar placeholder | `img/avatar-placeholder.png` | Verificar | Substituir se necessário |
| Logo/UI | criar novo | Original | Produzir |

## Registro de licenças

| Asset | Fonte | Licença | Permite uso comercial | Permite modificar | Comprovante |
|---|---|---|---|---|---|
| hero video | TBD | TBD | TBD | TBD | TBD |

## Regras

- Vídeo e imagens grandes ficam fora do Git; usar CDN/object storage.
- Guardar comprovante de licença (URL, print, contrato).
- Adicionar disclaimer de não afiliação com Sony/Polyphony.
