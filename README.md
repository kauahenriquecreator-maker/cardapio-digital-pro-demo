# Cardápio Digital PRO — Brasa Burger (DEMO)

Projeto HTML/CSS/JavaScript sem framework, banco de dados ou dependência de build. **Brasa Burger é uma marca fictícia; preços e produtos são demonstrativos.**

## Abrir e testar
1. Extraia o ZIP.
2. Abra `index.html` no Chrome/Edge (com internet para carregar as fontes Google; sem internet usa fontes alternativas).
3. Teste categorias, busca, adicionar itens, alterar quantidades e conferir total.
4. Clique em **Configurar WhatsApp** e informe um **número comercial seu ou autorizado**, no formato `55` + DDD + número. O valor fica salvo somente no navegador.
5. Monte um pedido e clique em **Enviar pedido no WhatsApp**. Confira a mensagem aberta e **só envie para um número que tenha autorizado o teste**.

## Publicação gratuita — GitHub Pages
1. Crie um repositório público no GitHub (ex.: `cardapio-demo`).
2. Faça upload dos três arquivos (`index.html`, `styles.css`, `app.js`) na raiz do repositório.
3. Em **Settings > Pages**, selecione **Deploy from a branch**, branch `main`, pasta `/ (root)` e salve.
4. Aguarde a publicação e abra a URL informada pelo GitHub Pages. Os nomes exatos de botões podem mudar.
5. No celular, configure o WhatsApp e teste a navegação. **A configuração do número não é compartilhada entre visitantes ou dispositivos.** Antes de entregar a um cliente, configure o número autorizado diretamente no código ou use uma configuração hospedada adequada (veja abaixo).

## Para publicar um cardápio real para um cliente
- Substitua marca, textos e itens no `index.html` e no array `PRODUCTS` em `app.js`.
- **IMPORTANTE:** este protótipo salva o telefone somente no `localStorage` do navegador. Para que TODOS os clientes enviem pedidos ao estabelecimento, substitua a linha `let phone = storage.get('brasa-phone-v1','');` por `let phone = '55DDDNUMEROAUTORIZADO';` com o número comercial real autorizado. Opcionalmente, remova o botão de configuração pública e o diálogo de configuração antes da entrega.
- Hospede em uma conta controlada pelo cliente ou formalize quem será responsável por hospedagem e domínio.
- Use fotos próprias/licenciadas, revise preços, disponibilidade, entrega, horário e política de privacidade aplicável.
- Teste um pedido real **com autorização do estabelecimento** antes de anunciar como operacional.

## Limites da versão 1
- Não recebe pagamentos, não calcula frete, não verifica estoque e não confirma pedidos automaticamente.
- Carrinho, nome, observações e configuração são locais ao navegador; não há servidor, painel administrativo ou sincronização.
- O clique abre o WhatsApp com a mensagem preenchida; **o usuário precisa confirmar o envio**.
- O checkout não garante que a loja esteja aberta, nem que haja entrega disponível.
- Emojis são ilustrações, não fotos reais dos produtos.

## Estrutura
- `index.html`: conteúdo e componentes da página.
- `styles.css`: identidade visual e responsividade.
- `app.js`: produtos, categorias, busca, carrinho, persistência local e WhatsApp.

## Checklist antes da venda
[ ] Testar no Android e no notebook
[ ] Conferir preço, nome e descrição de cada produto
[ ] Configurar número comercial autorizado para todos os visitantes
[ ] Testar abertura do WhatsApp e envio com autorização
[ ] Formalizar escopo, prazo, alterações, suporte, hospedagem e preço
[ ] Não alegar aumento de faturamento sem evidências
