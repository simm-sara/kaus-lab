# Kaus Lab — hub

Página única de apresentação da Kaus Lab: quem sou, por que a Kaus Lab existe e os projetos (Portfólio e Música).

- `index.html`: o site inteiro (HTML, CSS e JS num arquivo só; o objeto 3D usa Three.js via CDN).
- `previews/`: screenshots de referência. Não vão para o site.
- `.github/workflows/pages.yml`: publica o site no GitHub Pages a cada push na `main`.

## Publicar

1. Faça o merge desta branch na `main`.
2. No GitHub: **Settings → Pages → Build and deployment → Source: GitHub Actions**.
3. O site sobe em `https://<usuario>.github.io/kaus-lab/` a cada push na `main`.

## Domínio próprio

1. Crie um arquivo `CNAME` na raiz do repo com o domínio, uma linha só (ex.: `kauslab.com`).
2. No painel onde o domínio foi comprado, crie os registros DNS:
   - Domínio raiz (`kauslab.com`): quatro registros **A** apontando para
     `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - `www`: um registro **CNAME** apontando para `<usuario>.github.io`
3. Em **Settings → Pages**, preencha o domínio e marque **Enforce HTTPS** quando liberar.

## Easter egg

O e-mail ainda é um placeholder. Clicar nele embaralha o texto; digitar `kaus` em qualquer lugar da página dispara uma "reação" no objeto do topo. Quando o e-mail existir, troque o `<button class="mail">` por um link `mailto:`.
