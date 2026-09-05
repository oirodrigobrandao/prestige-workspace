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
  - **Atenção com colunas estreitas (ex: layout de foto 56%/44% com texto de um lado):** a Mirano Extended é uma fonte larga — em colunas de ~380-450px de largura, títulos com 6+ palavras ou palavras longas ("equipamento", "arranque", "embreagem") frequentemente quebram em palavra isolada mesmo com `text-wrap: balance` ligado (o balance só equilibra o comprimento das linhas, não evita viúva). Sempre **renderizar e olhar o PNG** antes de aprovar um título nessa coluna. Se aparecer palavra isolada: 1) encurtar a frase, 2) mover o título pra um layout de largura cheia (~950px, como o padrão de citação em tela cheia), ou 3) reduzir o font-size — nessa ordem de preferência.

---

## Estilo geral

A identidade visual da Prestige é REAL e MOVIMENTADA. A regra de ouro é **Documentar em vez de Criar**.
A fotografia deve ser clara/real, enquanto o design gráfico (chanfros, cores preto/dourado, tarjas de texto) será sobreposto a ela.

**Direção de Arte Fotográfica (JSON obrigatório para Magnific/IA):**

```json
{
  "estilo_geral": {
    "tipo": "Fotografia real e documental",
    "estetica": "Oficina de bairro premium, organizada, movimentada, humana",
    "iluminacao": "Luz natural de dia nublado ou luz fria de lâmpadas LED de galpão. Fotos 'cruas' sem edição pesada.",
    "grau_de_perfeicao": "Imperfeito e autêntico. Sujeira, marcas de pneu, água no chão, ferramentas fora do lugar.",
    "referencias_visuais": "Piso de concreto com faixas amarelas, telhado metálico escuro, portão de aço, estrutura de tijolo cinza, refletores industriais."
  },
  "elementos_permitidos": [
    "Funcionários reais trabalhando (uniformes pretos da Prestige, bonés) de forma natural e espontânea",
    "Carros reais de clientes (sem brilho extremo de showroom, com poeira ou sujeira de uso diário)",
    "Ferramentas reais, mangueiras, elevadores hidráulicos, prateleiras com produtos, poltronas de espera",
    "Chão molhado, espuma de sabão, reflexos reais da luz no piso",
    "Enquadramentos amadores estilo foto de celular (ângulos levemente tortos, profundidade de campo média, sem simetria perfeita)"
  ],
  "elementos_proibidos": [
    "Cenários de estúdio com fundo infinito preto ou branco",
    "Iluminação dramática de cinema (neon, alto contraste extremo, sombras profundas demais)",
    "Carros com pintura 'vitrificada' sintética de IA, sem nenhuma sujeira ou marca de uso real",
    "Ilustrações, renderizações 3D ou qualquer coisa que pareça gráfico/CGI",
    "Decorações de inauguração (bolas amarelas e pretas, faixas comemorativas)",
    "Fundos desfocados de palmeiras, prédios futuristas ou paisagens genéricas de IA",
    "Pessoas com rostos perfeitos demais ou poses robóticas",
    "Logos, marcas ou uniformes de concorrentes",
    "Cenário externo com cara de subúrbio americano (gramado aparado, casas de madeira estilo New England, fiação subterrânea) quando o post não é sobre outro país — mesmo em posts sem oficina (ex: carro na rua ao entardecer), o ambiente precisa parecer uma rua brasileira real: fiação aérea emaranhada, muros residenciais simples, asfalto com remendos. (Confirmado em 05/09/2026 no carrossel de 06/09: imagens de carro em rua ficaram com cara de bairro americano)",
    "Carro exageradamente limpo/intacto num post que não é sobre estética automotiva — mesmo fora da oficina, o carro de rua deve ter poeira e marcas de uso reais, não brilho de carro zero km"
  ],
  "regra_de_humanizacao": {
    "descricao": "Sempre que o post for sobre serviço, oficina ou lava jato, DEVE haver pelo menos um funcionário da Prestige em cena (mãos, braços, rosto) realizando uma tarefa real.",
    "uso_de_clonagem": "Usar as fotos reais de funcionários (Fernando, Erick, equipe) para clonar a aparência e os traços no Magnific antes de gerar."
  }
}
```

> **Dica para uso de IA (Magnific/Midjourney):** Ao invés de pedir para criar a cena do zero, use uma foto real da oficina (ex: de `dados/midia-bruta/`) como base. Instrua o modelo a usar a foto real como Image Prompt (referência) e pedir para "renderizar em altíssima qualidade mantendo 100% da identidade, removendo decoração de inauguração e adicionando leve granulação de foto de celular". Use a IA apenas para aumentar resolução (upscale) ou estender fundo, preservando a essência da oficina real.

---

## Elementos-chave

- **Chanfro (corte diagonal no canto):** o elemento mais recorrente da marca. Caixas de texto, listas de serviço, tarjas de preço, botões de contato e QR code sempre têm um canto (geralmente superior-direito ou inferior-direito) cortado na diagonal, formando um paralelogramo/seta em vez de retângulo puro. Esse recorte é o que "amarra" qualquer peça ao visual da marca — usar sempre que possível em blocos de destaque
- Bordas: retas, sem arredondamento — reforça o caráter técnico/angular da marca e do logo
- Border-radius dos cards: zero
- **Não existe "padrão visual B" com cantos arredondados/pills.** Todo carrossel (independente do tom — educativo, institucional, reflexivo) usa o mesmo sistema "Editorial Chanfrado": cantos retos, chanfro nas tarjas/cards, zero border-radius em qualquer bloco de conteúdo. (Corrigido em 05/09/2026: o carrossel de 06/09 tinha sido feito com cards arredondados e tags em pill — fora do design-guide — e precisou ser refeito do zero.)
- **Contraste de texto sobre foto:** fotos reais/documentais (com luz de dia ou LED de galpão) costumam ficar mais claras que uma foto de estúdio. O overlay escuro (gradiente preto) precisa ter opacidade mínima de ~0.55–0.8 exatamente nas áreas onde cai texto branco — não usar o mesmo gradiente "padrão" sem checar contra a foto real usada. Sempre adicionar um `text-shadow` sutil no `h1` (algo como `0 2px 14px rgba(0,0,0,0.85)`) como reforço de legibilidade, e olhar o PNG renderizado antes de aprovar.
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
- **Slide final de carrossel (CTA/contato):** foto grande em cima + bloco dourado sólido embaixo com os itens de contato (mensagem, localização, tipo de avaliação) e rodapé (@handle + logo). Dimensionar a altura do bloco dourado pelo conteúdo real (itens + divisor + rodapé, com uma margem curta entre os dois), nunca deixar `justify-content: space-between` esticar um bloco de altura fixa grande — isso cria espaço vazio no meio. Referência de proporção validada: foto ~970px / bloco dourado ~380px numa arte de 1080x1350.

---

## O que NUNCA fazer

- **Prova social nunca leva imagem de IA nem foto genérica de banco/stock — em nenhum slide, principalmente na capa.** Posts de prova social, depoimento ou "caso real" só podem usar fotos genuinamente reais daquele atendimento específico (do Erick ou do banco de mídia da Prestige em `dados/midia-bruta/`). Não vale gerar via Magnific "parecendo real", não vale reaproveitar imagem de outro post editorial genérico com crop diferente fingindo ser aquele caso, e não vale usar foto de banco de imagens de terceiros que não é da Prestige. Se não existir foto real do caso, **parar e avisar o usuário** pedindo a mídia real — nunca simular a prova. (Confirmado em 01/09/2026 depois de 3 posts — dias 20, 05 e 12/09 — descobertos usando imagem fabricada ou de terceiros em post de prova social.)
- Não distorcer o wordmark "PRESTIGE" nem separar do bloco "AUTO SPA" sem necessidade
- Não usar paleta de cores fora de preto/branco/dourado em materiais oficiais
- Não usar fontes arredondadas ou "amigáveis demais" que destoem do estilo angular da marca
- Não usar ilustração no lugar de fotografia real nos materiais de serviço/promoção
- Não exibir logos, nomes ou uniformes de marcas terceiras/concorrentes em fotos ou criativos gerados (usar vestimentas limpas/lisas ou a marcação Prestige)
- Não usar caixas/botões com cantos 100% retos sem o chanfro em peças de destaque — foge do padrão observado
- Não deixar nenhum modelo de IA "desenhar" o logo ou o monograma "P" da marca dentro da imagem gerada — IA generativa não reproduz o wordmark com precisão (recriou o "PRESTIGE" numa fonte genérica e separou o "AUTO SPA" do bloco dourado no primeiro teste real, em 31/08/2026). Deixar espaço negativo limpo na composição e sobrepor o arquivo real depois (`marca/PNG/Prestige Auto Spa-06.png` fundo escuro, `-07.png` fundo dourado, `-10.png` monograma isolado)
- A regra anti-viúva (linha 30) vale também pra títulos gerados por IA, inclusive quando a palavra final é um "reveal"/palavra de efeito em destaque — nunca isolar sozinha numa linha, mesmo com cor diferente

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
