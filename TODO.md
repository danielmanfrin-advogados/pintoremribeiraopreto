# Entregas

## Estrutura estática e configuração
- [ ] As páginas existem como HTML real em `/`, `servicos/` com 3 rotas, `bairros/` com 6 rotas, `/sobre/`, `/perguntas-frequentes/` e `/politica-de-privacidade/`.
- [ ] O projeto usa somente HTML, CSS e JavaScript puros, com um `style.css`, `config.js` e `tracker.js` compartilhados.
- [ ] `package.json` não possui `dependencies` nem `devDependencies`; `build.js` copia a raiz para `dist`; `vercel.json` usa `npm run build`, saída `dist`, `cleanUrls: true` e `trailingSlash: true`.

## Conversão e rastreamento
- [ ] Todos os botões WhatsApp usam `data-acao="whatsapp"`, `data-local`, `data-msg` e número inicial provisório; todos os botões de telefone usam `data-acao="ligar"` e `data-local`.
- [ ] `config.js` concentra os números, mensagem padrão, nicho, cidade e endpoint, e trocar os números altera todas as páginas.
- [ ] `tracker.js` envia os campos de clique ao Apps Script por GET com `fetch` no-cors e fallback de imagem, sem coletar nome, e-mail, CPF ou cookies de publicidade.

## Conteúdo, design e acessibilidade
- [ ] A inicial tem navegação flutuante, hero com foto, selo, H1, subtítulo, WhatsApp, telefone, barra de pedido rápido, boas-vindas, 3 cards, 4 diferenciais, bairros, FAQ, CTA final, rodapé e barra fixa mobile.
- [ ] As páginas de serviço têm breadcrumb, H1, imagem, descrição útil e única com pelo menos 250 palavras, dúvidas próprias, bairros, links internos e CTA final.
- [ ] As páginas de bairro têm breadcrumb, H1, pelo menos 150 palavras próprias, situações alternadas e links internos sem inventar fatos locais.
- [ ] O aviso legal obrigatório aparece no rodapé de todas as páginas.
- [ ] O layout é mobile first, sem scroll horizontal em 360 px, com foco visível, contraste AA, alvos de toque de 44 px e respeito a `prefers-reduced-motion`.

## SEO e GEO
- [ ] Cada página tem title até 60 caracteres, meta description de 120 a 155 caracteres, canonical absoluto, Open Graph, Twitter Card, `lang="pt-BR"`, favicon e `robots index,follow`.
- [ ] JSON-LD válido usa WebSite na inicial, Service nas páginas de serviço e bairro, FAQPage onde as perguntas aparecem e BreadcrumbList nas internas.
- [ ] `sitemap.xml` lista as 13 páginas com lastmod e prioridades; `robots.txt` libera rastreamento; `llms.txt` resume serviços, bairros, páginas institucionais e FAQs.

## Imagens e documentação
- [ ] `img/` contém hero 16:9, sobre 4:3 e uma foto 4:3 por serviço, com alt neutro e sem texto, marcas ou rostos destacados.
- [ ] `apps-script/Code.gs` é o script fornecido no briefing e `LEIA-ME.txt` explica números, planilha, Search Console, sitemap e substituição de imagens.
