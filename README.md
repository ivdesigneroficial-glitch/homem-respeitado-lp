# Biblioteca do Homem Respeitado — Landing Page

Página de vendas da coleção de 10 ebooks (@homemrespeitadobr).

## Estrutura
- `index.html` — página completa (HTML + CSS + JS em arquivo único)
- `assets/capas/1.jpg` … `10.jpg` — capas dos livros
- `.nojekyll` — garante que o GitHub Pages sirva os arquivos como estão

## Publicar no GitHub Pages
1. Suba os arquivos no repositório
2. Settings → Pages → Source: `Deploy from a branch`
3. Branch: `main` / pasta `/ (root)` → Save
4. Em ~1 minuto a página fica no ar em `https://SEU-USUARIO.github.io/NOME-DO-REPO/`

## Ligar o botão de compra à Kiwify
No `index.html`, procure por `href="#"` (são 2 botões) e por `href="#comprar"` (2 botões de navegação).
Troque apenas os `href="#"` pelo link de checkout da Kiwify:

```html
<a href="https://pay.kiwify.com.br/SEU-LINK" class="cta">Comprar agora — acesso imediato</a>
```

Os `href="#comprar"` devem continuar como estão — eles só rolam a página até a seção de preço.
