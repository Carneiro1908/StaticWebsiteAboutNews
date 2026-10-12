# Aveiro em Crescimento: como publicar o site

Site estático (HTML + CSS). Não precisa de servidor, base de dados nem build.

## Estrutura

```
aveiro-site/
  index.html
  styles.css
  fotos/          <- coloque aqui as suas fotografias
  README.md
```

## Fotografias

Cada espaço tracejado no site indica o nome do ficheiro esperado (por exemplo `fotos/rossio-depois.jpg`). Basta guardar a imagem na pasta `fotos/` com esse nome. Quando o ficheiro existe, aparece automaticamente no lugar do espaço reservado.

Dicas:
- Use JPG ou WebP, com cerca de 1600 px de largura e menos de 400 KB cada.
- Preencha as legendas (`<figcaption>`) com local, autor e data.
- Use apenas fotografias suas ou com licença que permita a reutilização (por exemplo Wikimedia Commons, com crédito). Não copie imagens de notícias.

## Onde alojar

Por ser um site estático, o Render funciona, mas há opções mais adequadas:

| Opção | Custo | Porquê |
|---|---|---|
| **Cloudflare Pages** (recomendado) | Grátis | Rápido, sem "adormecer", domínio próprio fácil |
| **Netlify** | Grátis | Arrastar a pasta e publicar em segundos |
| **GitHub Pages** | Grátis | Ótimo se já usa GitHub |
| **Render (Static Site)** | Grátis | Funciona bem como site estático; evite o tipo "Web Service" para isto |

O Render só compensa se mais tarde precisar de back-end (formulários, comentários, base de dados).

### Netlify (o mais rápido)
1. Vá a app.netlify.com/drop.
2. Arraste a pasta `aveiro-site` inteira.
3. O site fica online com um endereço `.netlify.app`.

### Cloudflare Pages
1. Crie conta em pages.cloudflare.com.
2. "Create project" → "Upload assets" → arraste a pasta.
3. Opcional: associe um domínio próprio.

### GitHub Pages
1. Crie um repositório e envie os ficheiros.
2. Settings → Pages → Branch `main` → pasta `/ (root)`.

### Render (Static Site)
1. Envie os ficheiros para um repositório no GitHub.
2. Render → New → **Static Site** → escolha o repositório.
3. Build command: deixe vazio. Publish directory: `.`

## Antes de publicar

- Confirme os números do INE (os valores de 2021 usados são preliminares).
- Troque a lista de fontes por links diretos para cada documento.
- Acrescente os dados do concelho que quiser destacar (alojamento local, rendas, estudantes).
