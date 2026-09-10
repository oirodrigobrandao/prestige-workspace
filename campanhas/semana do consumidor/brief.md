# Semana do Consumidor Prestige — Brief da campanha

Ponto único de referência desta campanha. Tudo que precisa ser decidido, calculado ou produzido está aqui — não precisa reabrir os áudios ou o catálogo de novo.

## Resumo

- **Nome da campanha:** Semana do Consumidor Prestige
- **Chamada:** descontos de até 50%
- **Produto da campanha:** "Prestige Full" — pacote fechado por porte (P, M, G, GG), não é desconto item por item
- **Composição do Prestige Full** (conforme áudio do Erick): soma de 3 produtos do catálogo, do mesmo porte:
  1. **Combo Prestige** (já inclui lavagem completa, higienizações e polimento de pintura)
  2. **Vitrificação** (seção "Proteção e Acabamento" do catálogo — já inclui o polimento técnico prévio, por isso não soma o polimento separado)
  3. **Restauração de Farol** (valor único, não varia por porte)
- **Desconto:** 35% aplicado em cima da **soma dos três**, ignorando os descontos máximos individuais de cada item na tabela (20%/45%). Confirmado por Erick em 2 áudios diferentes ("esquece os descontos que já tá, do valor que já tá aí, tu aplica 35%").

## Tabela Prestige Full (calculada)

| Porte | Combo Prestige | Vitrificação | Restauração de Farol | Soma (De) | Desconto 35% | Valor final (Por) |
|---|---|---|---|---|---|---|
| P | R$ 1.292,00 | R$ 1.500,00 | R$ 496,25 | R$ 3.288,25 | R$ 1.150,89 | **R$ 2.137,36** |
| M | R$ 1.421,00 | R$ 1.625,00 | R$ 496,25 | R$ 3.542,25 | R$ 1.239,79 | **R$ 2.302,46** |
| G | R$ 1.550,00 | R$ 1.750,00 | R$ 496,25 | R$ 3.796,25 | R$ 1.328,69 | **R$ 2.467,56** |
| GG | R$ 1.679,00 | R$ 1.835,00 | R$ 496,25 | R$ 4.010,25 | R$ 1.403,59 | **R$ 2.606,66** |

Farol usa sempre R$ 496,25 (Restauração de Farol), porque essa é a única linha de farol do catálogo com esse nome — o valor "300 e pouco" que o Erick citou no terceiro áudio foi um exemplo aproximado ("que é um exemplo"), não o valor real. Se ele quis dizer Clareamento de Farol (R$ 100,00) em vez de Restauração, ajustar a tabela é rápido — mas o mais provável, pelo contexto de "revitalização do farol", é Restauração mesmo.

⚠️ Nota: a chamada de marketing é "até 50%" mas o cálculo real dá 35% de desconto em todos os portes. Vale alinhar com Erick se o "até 50%" é só a chamada de campanha (arredondamento comercial) ou se algum porte/serviço específico deveria realmente bater 50%.

## Confirmado

- [x] Desconto: 35% flat sobre a soma dos 3 produtos, todos os portes
- [x] Escopo do pacote: Combo + Vitrificação + Restauração de Farol (não é a lista solta de serviços — apesar da mensagem inicial falar "lavagem de carroceria, chassis, motor, banco, teto, polimento, vitrificação, revitalização de farol", tudo isso já está dentro do Combo + Vitrificação, então o Prestige Full cobre a "boba toda" num pacote só)
- [x] Estilo visual: replicar o formato de referência (`referencia visual.jpeg`, print InfinitePay) como está — preço "De/Por" gigante + badges em pílula com cantos arredondados ao redor, mesmo sendo exceção ao padrão de chanfro do `marca/design-guide.md`. Documentando aqui pra essa exceção não ser "corrigida" por engano depois.
- [x] Peças por porte: Erick pediu explicitamente "faz um monte de banner diferente, com P, com M, com G" — ou seja, uma peça (banner) pra cada porte, não uma peça genérica.

## Pendente (precisa de você)

- [ ] Confirmar com Erick se farol = Restauração (R$ 496,25) ou Clareamento (R$ 100,00)
- [ ] Confirmar se GG também entra nos banners (áudio só cita P, M, G) ou se fica de fora da campanha
- [ ] Decidir o formato de publicação final: os "banners" viram um carrossel único (1 slide por porte), posts avulsos separados, ou só artes de banner pra story/destaque? O áudio descreve a peça (banner com preço De/Por) mas não o formato de postagem no Instagram.
- [ ] Data de início/fim da campanha (nenhum áudio menciona prazo)

## Insumos brutos (na mesma pasta)

- `WhatsApp Audio 2026-09-10 at 12.07.15.opus` — explicação original da lógica do Prestige Full
- `WhatsApp Audio 2026-09-10 at 12.44.10.opus` — reforço do desconto de 35%
- `oferta WhatsApp Audio 2026-09-10 at 13.17.03.opus` — exemplo de cálculo (valores aproximados, não usar como fonte de preço)
- `transcricoes_audios.md` — transcrição completa dos 3 áudios acima
- `Catalogo- Prestige Auto Spa.pdf` — catálogo de preços oficial (mesmas tabelas coladas nesta conversa)
- `referencia visual.jpeg` — referência de estilo visual (print InfinitePay)

## Testes de criativo

Peças por porte (P/M/G/GG), em duas versões: **Feed** (4:5) e **Stories** (9:16). Testando um criativo primeiro (porte P, Feed) antes de replicar pros demais.

- `testes/prestige-full-P-feed-v1.jpg` — gerado no Magnific, com foto real da Prestige como referência de marca (box de lavagem real, carro real). Layout limpo: 2 pills acima do carro, 3 pills abaixo, preço e desconto à direita. **Sem bugs.**
- `testes/prestige-full-P-feed-v2.jpg` — mesma geração, variação 2. Bug: o pill "Lavagem completa" aparece duplicado (sozinho no topo e de novo na fileira de baixo). Descartar ou regenerar se preferir esse layout.
- `testes/prompt-gpt.md` — prompt equivalente pra testar a mesma peça no GPT, pra comparar qualidade/estilo antes de bater o martelo em qual ferramenta usar pros outros 7 criativos restantes (M, G, GG × Feed, Stories).

### Porte M (novo padrão, a partir da sua peça manual no Figma)

Você desenhou a versão do Porte P direto no Figma (não deu pra puxar o arquivo — Figma pessoal não vinculado à conta conectada, `rodrigo.brandao@housi.com.br`; se quiser que eu edite direto no Figma depois, é só compartilhar o arquivo com esse e-mail). Recriei o mesmo padrão em HTML/CSS com os dados do M, usando uma foto real da Prestige (`dados/midia-bruta/conteudo-diario/jpg_converted/IMG_0400.jpg` — funcionário real + BMW real + placa com a marca) em vez de foto de banco de imagem.

- `testes/prestige-full-M-feed.html` — código-fonte editável (fácil de gerar G e GG só trocando os valores e a porte)
- `testes/prestige-full-M-feed.png` — render final 1080x1350

⚠️ Nota de marca: o botão de CTA e o texto "Economia de R$..." usam verde, que não é uma das 3 cores oficiais (preto/branco/dourado) do `marca/design-guide.md`. Mantive porque veio da sua peça original — avisa se quiser trocar pra dourado.

Próximo passo: você aprova o padrão do M (ou pede ajuste) e aí eu gero G e GG no mesmo molde, e depois as versões Stories (9:16) dos 4 portes.

## Próximos passos por fase

1. **Fechar briefing** — resolver o checklist "Pendente" acima (farol, GG dentro ou fora, formato de publicação, datas)
2. **Escrever textos/legendas** — usar skill `carrossel` se o formato final for carrossel; texto avulso se forem banners/posts independentes
3. **Produzir visual** — adaptar a referência InfinitePay pro preto/dourado/branco da Prestige, badges em pílula (exceção aprovada), um banner por porte com a tabela acima
4. **Aprovação do Erick** — validar valores e arte antes de publicar
5. **Publicação/agendamento**
