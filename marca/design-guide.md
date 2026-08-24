# Guia de Design — Prestige Auto Spa

> Você pode editar esse arquivo a qualquer momento.
> As skills de carrossel, proposta e slide leem este arquivo antes de criar qualquer visual.

---

## Cores

- **Fundo principal:** branco (#FFFFFF)

- **Cor de destaque / CTA:** dourado — `#CC9933` (extraído direto do arquivo do logo, `marca/PNG/Prestige Auto Spa-07.png`)

- **Texto principal:** preto (#000000)

- **Fundo alternativo / cards:** dourado sólido (mesma cor de destaque), usado em variações do logo — pode servir de fundo alternativo em peças de maior impacto

- **Cor proibida:** cores fora da paleta preto/branco/dourado — evitar paletas coloridas genéricas que destoem do posicionamento premium

---

## Tipografia

- **Títulos e destaques:** Mirano Extended (arquivo em `marca/Tipografia/`) — fonte angular, condensada/extended, usada no próprio logo. Pesos disponíveis: Thin, Light, Regular, Medium, SemiBold, Bold (+ itálicos)

- **Corpo, subtítulos e botões:** a definir — Mirano Extended é uma fonte de display (boa pra títulos/wordmark), recomenda-se uma sans-serif neutra pra textos longos até a marca definir uma fonte de corpo oficial

- **Peso do título:** Bold ou SemiBold

- **Regra de diagramação e quebra de linhas (Anti-viúvas):** Nunca permitir uma palavra isolada sozinha em uma linha nos títulos, subtítulos ou chamadas de destaque. Distribuir as palavras de forma equilibrada e organizada através de quebras manuais semânticas (`<br>`), agrupando termos lógicos (ex: 2 a 4 palavras por linha com comprimentos harmônicos). Usar `text-wrap: balance` e espaçamentos não-quebráveis (`&nbsp;`) sempre que apropriado.

---

## Estilo geral

Moderno, angular e premium — estética automotiva/tech. Fundo predominantemente preto, com fotografia real de carros e dos serviços sendo executados (nunca ilustração) — muitas vezes com iluminação dramática/alto contraste. Visual limpo, direto, sem poluição visual.

> Baseado nos 7 materiais (banners, adesivos, posts) que o Erick já produziu e passou como referência em 23/07/2026 — é o mais próximo de um padrão que a marca tem hoje, mas **ainda não foi oficializado com o Erick**. Tratar como ponto de partida pra propor o padrão do item "Arte padrão de preços/serviços" em `tarefas.md`, não como regra fechada.

---

## Elementos-chave

- **Chanfro (corte diagonal no canto):** o elemento mais recorrente da marca. Caixas de texto, listas de serviço, tarjas de preço, botões de contato e QR code sempre têm um canto (geralmente superior-direito ou inferior-direito) cortado na diagonal, formando um paralelogramo/seta em vez de retângulo puro. Esse recorte é o que "amarra" qualquer peça ao visual da marca — usar sempre que possível em blocos de destaque
- Bordas: retas, sem arredondamento — reforça o caráter técnico/angular da marca e do logo
- Border-radius dos cards: zero
- Botões / tarjas de contato: bloco branco ou dourado sólido com o chanfro, texto em preto bold (número de telefone sempre em destaque)
- Listas de serviço: caixas com borda fina dourada (outline, fundo preto) e o mesmo corte diagonal, uma abaixo da outra
- Selo/badge de serviço: emblema circular (coroa + grinalda/laurel, estilo brasão) usado pra marcar categorias/tiers de serviço (ex: "Prestige Wash Essencial") — dourado e branco sobre fundo escuro
- QR code: sempre em bloco branco, chanfrado, geralmente ao lado do contato — usado pra direcionar pro Instagram ou agendamento
- Sombras: evitar sombras pesadas — manter visual clean, contraste vem da cor e da foto, não de efeito

---

## Layouts recorrentes

- **Banner horizontal (loja/parceiro):** foto do serviço à esquerda, lista de serviços chanfrada ao centro, bloco de contato (telefone + horário) chanfrado à direita
- **Post/story de oferta:** foto do carro em destaque, preço grande em tarja dourada chanfrada, QR code, endereço no rodapé
- **Flyer vertical (impresso):** foto no topo (metade da peça), lista de serviços chanfrada + QR code na parte inferior preta
- **Adesivo/etiqueta de controle** (ex: troca de óleo): fundo claro (branco/creme), faixa dourada de destaque, campos pra preencher à mão, contato no rodapé
- **Post Instagram (institucional/marco):** foto dramática do carro, texto de destaque em branco + número grande em dourado com efeito de textura, sem lista de serviços — usado pra marcos da marca (ex: 1.000 seguidores)

---

## O que NUNCA fazer

- Não distorcer o wordmark "PRESTIGE" nem separar do bloco "AUTO SPA" sem necessidade
- Não usar paleta de cores fora de preto/branco/dourado em materiais oficiais
- Não usar fontes arredondadas ou "amigáveis demais" que destoem do estilo angular da marca
- Não usar ilustração no lugar de fotografia real nos materiais de serviço/promoção
- Não exibir logos, nomes ou uniformes de marcas terceiras/concorrentes em fotos ou criativos gerados (usar vestimentas limpas/lisas ou a marcação Prestige)
- Não usar caixas/botões com cantos 100% retos sem o chanfro em peças de destaque — foge do padrão observado

---

## Logo

- **Arquivo (fundo claro, preto):** `marca/PNG/Prestige Auto Spa-01.png` (horizontal) / `Prestige Auto Spa-02.png` (empilhado)
- **Versão pra fundo escuro (branco):** `marca/PNG/Prestige Auto Spa-06.png` (horizontal, confirmado por checagem de pixel em 24/08/2026) / `07.png` (variações sobre fundo dourado). **Atenção:** `Prestige Auto Spa-05.png` apesar do nome sugerir "fundo escuro", na prática tem as letras pretas (igual ao -01) — não usar em fundo escuro/dourado, fica ilegível. Confirmar visualmente antes de usar qualquer arquivo de logo novo.
- **Monograma / ícone:** `marca/PNG/Prestige Auto Spa-10.png` (letra "P" dourada, isolada)
- **Onde usar:** slide final do carrossel (CTA), header de propostas, slides de apresentação, materiais pra parceiros
- **Tamanho sugerido:** largura entre 120-200px nos HTMLs

---

## Perfil do autor

> Usado no estilo "tweet" do carrossel. Preenchido automaticamente no setup.

- **Nome:** Prestige Auto Spa
- **Handle:** @prestigeautospaof
- **Foto:** *(a definir — usar logo ou monograma enquanto não houver foto de perfil específica)*
- **Badge verificado:** não

---

## Observações adicionais

Fotos e vídeos brutos disponíveis em `dados/midia-bruta/` (`inauguracao/`, `conteudo-diario/`, `diversos/`) — pasta local, fora do GitHub por ser muito pesada (~1,5GB). Ao usar uma peça específica, processar pontualmente (still, corte, etc.) e salvar o resultado fora dessa pasta.

Os 7 materiais de referência usados pra descrever o padrão acima (banners, adesivos, posts) foram compartilhados só no chat — ainda não estão salvos em arquivo. Recomendo salvar em `marca/referencias/` pra servirem de exemplo real quando uma skill for gerar uma peça nova.
