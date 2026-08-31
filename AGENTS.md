# Prestige Auto Spa — instruções pra qualquer agente (cross-tool)

Este arquivo existe pra ferramentas que não leem `CLAUDE.md` nativamente (ex: Antigravity/Gemini) — mas o conteúdo abaixo vale pra qualquer agente que trabalhe neste projeto.

**Antes de gerar qualquer texto, imagem ou peça visual pra Prestige Auto Spa, ler primeiro:**

1. `CLAUDE.md` — quem é o negócio, estrutura de pastas, tom de voz
2. `marca/design-guide.md` — cores, tipografia, layout, o que nunca fazer

Esses dois arquivos são a fonte da verdade. Não duplicar o conteúdo deles aqui — só reforçar abaixo os pontos que já causaram erro real numa geração de imagem, pra não repetir.

## Gerar imagens com IA (Nano Banana, Imagen, ou qualquer modelo)

- Sempre usar como referência pelo menos uma foto real do ambiente/carro/equipe da Prestige (`sites-landing-pages/imgs-prestige/` ou `dados/midia-bruta/`) — mesma regra que já vale pro Magnific em `CLAUDE.md`.
- Nunca deixar o modelo desenhar o logo ou o monograma "P" da marca — ver `marca/design-guide.md`, seção "O que NUNCA fazer".
- A regra anti-viúva de tipografia (`marca/design-guide.md`, seção Tipografia) é obrigatória mesmo em título gerado por IA.

## Aprendizado registrado em 2026-08-31

Primeiro teste real de geração via Antigravity (carrossel `2026-09-16-polimento-tecnico-holograma`): fotorrealismo muito bom, mas caiu nos dois pontos acima em 2 dos 6 slides — por isso viraram regra explícita no design-guide, não só recomendação implícita.

## Funcionário em imagem gerada por IA

Priorizar sempre clonar/manter a aparência de um funcionário real, usando como referência as fotos em `sites-landing-pages/imgs-prestige/` ou `dados/midia-bruta/`. Só usar um rosto fictício gerado pela IA quando não for possível clonar a pessoa real com consistência ou quando não existir imagem real dela no banco pra aquela cena/ângulo. (Regra definida em 2026-08-31 — ver `marca/design-guide.md`.)
