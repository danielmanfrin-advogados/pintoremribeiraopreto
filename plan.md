# Plano de implementação e design

## Escopo
Portal estático multipágina para captar pedidos de orçamento de pintura de casas, comércios e apartamentos em Ribeirão Preto. O conteúdo será em português do Brasil, com foco em SEO local e GEO, sem promessas de preço, prazo, garantia, avaliações ou dados empresariais inventados.

## Arquitetura
- HTML real em 13 rotas: inicial, 3 serviços, 6 bairros, Sobre, Perguntas frequentes e Política de privacidade.
- `style.css` compartilhado com layout mobile first, paleta creme e terracota, navegação flutuante, hero fotográfico, cards e barra fixa mobile.
- `config.js` concentra site, nicho, WhatsApp, telefone, cidade, mensagem padrão e endpoint.
- `tracker.js` ajusta os links e registra cliques com a lógica do briefing.
- `img/` contém `hero.jpg`, `sobre.jpg` e uma foto para cada serviço.
- `build.js`, `package.json` sem dependências e `vercel.json` geram `dist/` para Vercel.
- `sitemap.xml`, `robots.txt`, `llms.txt`, JSON-LD e breadcrumbs cobrem SEO/GEO.

## Direção visual escolhida
**Movimento:** editorial orgânico de bairro, com a sensação de uma recomendação local bem organizada.

**Princípios:** acolhedor, direto, legível e confiável. A conversão acontece por meio de escolhas curtas e botões sempre visíveis.

**Filosofia de cor:** creme para reduzir ruído visual, terracota profundo para comunicar trabalho manual e proximidade, verde para a ação de WhatsApp e carvão para telefone e rodapé.

**Paradigma de layout:** hero amplo com conteúdo alinhado à esquerda, barra de pedido sobreposta, seções alternadas e cards com imagens como pontos de pausa visual.

**Elementos de assinatura:** navegação em pílula, selo circular “Atendimento local” e faixas de CTA arredondadas.

**Interação:** microinterações discretas em hover e foco visível; a interface deve parecer simples antes de parecer tecnológica.

**Animação:** transições curtas apenas em cor, sombra e transformação; `prefers-reduced-motion` desativa rolagem suave e movimentos.

**Tipografia:** Fira Sans em pesos 400, 500, 600, 700 e 800, com fallback de sistema. H1 compacto, H2 editorial e corpo com leitura confortável.

**Essência:** um portal local que transforma uma dúvida de pintura em um pedido claro pelo WhatsApp. Personalidade: prático, cuidadoso, próximo.

**Voz:** frases curtas, sem exagero. Exemplos: “Diga o que precisa pintar e receba a orientação do prestador.” “O pedido começa com três informações simples.”

**Marca:** wordmark em negrito com um pequeno traço de pincel abstrato no favicon, sem tentar simular uma empresa específica.

**Cor proprietária:** terracota profundo `#9a3412`.
