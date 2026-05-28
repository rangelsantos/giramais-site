# MeuGanho Site

Site estatico publico do MeuGanho, pensado para GitHub Pages.

## Estrutura

- `index.html`: homepage com visao geral do app
- `privacy/index.html`: politica de privacidade publica com link direto
- `styles.css`: identidade visual alinhada ao tema Emerald do app
- `assets/logo-*.png`: versoes derivadas da arte oficial do MeuGanho para favicon, touch icon e uso visual no site
- `assets/favicon.ico`: favicon legado para navegadores
- `assets/og-image.png`: imagem para compartilhamento social
- `site.webmanifest`: manifesto web simples para publicacao
- `robots.txt`: instrucao basica para indexacao publica

## Publicar no GitHub Pages

1. Crie um repositorio GitHub para `meuganho-site`.
2. Envie estes arquivos para a branch `main`.
3. No GitHub, abra `Settings -> Pages`.
4. Em `Build and deployment`, selecione `GitHub Actions`.
5. O workflow `.github/workflows/deploy-pages.yml` fara o deploy automaticamente a cada push na `main`.
6. Aguarde o primeiro workflow concluir com sucesso.

URLs esperadas apos publicacao:

- Home: `https://SEU_USUARIO.github.io/meuganho-site/`
- Politica de privacidade: `https://SEU_USUARIO.github.io/meuganho-site/privacy/index.html`

## Observacoes

- Atualize o bloco de contato na pagina de privacidade se quiser incluir endereco comercial.
- Se for usar Google Play App Content -> Privacy Policy, informe a URL final da pagina `privacy/index.html`.
- O repositorio inclui `404.html`, `robots.txt`, `site.webmanifest` e workflow de Pages, ja prontos para publicacao.

## Estrutura de deploy automatizado

- `.github/workflows/deploy-pages.yml`: workflow oficial de build/deploy no GitHub Pages
- `404.html`: pagina de fallback com redirecionamento para a home
- `assets/logo-*.png`: tamanhos derivados da arte oficial do MeuGanho
- `assets/favicon.ico`: favicon legado
- `assets/og-image.png`: imagem para compartilhamento social
