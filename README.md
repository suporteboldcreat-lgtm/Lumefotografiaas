# LUME FILMES — landing page (projeto fictício de portfólio da Nuance)

Site estático: HTML, CSS e um JS mínimo. Sem framework, sem build, sem dependências.

## Como ver a página
Abra `index.html` no navegador (duplo clique). As fontes (Newsreader e Hanken Grotesk) vêm do Google Fonts e precisam de internet; sem elas, a página usa fontes do sistema.

## Estrutura
```
index.html        conteúdo e semântica
css/style.css     tokens (cores, escala tipográfica) e layout
js/main.js        configuração do WhatsApp
assets/img/       imagens (hoje: espaços reservados) e CREDITS.md
```

## 1. Conectar o WhatsApp (PENDENTE)
Abra `js/main.js` e preencha `whatsappNumber` com código do país + DDD + número, só dígitos
(formato de exemplo, não é número real: `5592900000000`). A mensagem pré-preenchida fica em `message`.
Com o número válido, os três botões abrem `wa.me` com a mensagem e o aviso de pendência some sozinho.
Enquanto estiver vazio, os botões levam ao bloco de contato e o aviso permanece visível.

## 2. Trocar as imagens de demonstração por fotos reais
Substitua os arquivos de `assets/img/` mantendo os nomes, ou edite os `<img>` do `index.html`.
Tamanhos de referência (largura): hero desktop 1920 (16:9) e 960; hero celular 900 (3:5) e 450;
manifesto 900 (3:4); portfólio 1 e 6: 1600; 2 e 5: 1000/900 (vertical); 3: 1500; 4: 900 (quadrada); abordagem 1920.
Exporte em WebP (qualidade ~75–80) e, para cada foto, uma versão com metade da largura.
Depois: atualize o `alt` de cada imagem para descrever a foto real, ajuste `width`/`height` se a proporção mudar,
confira o enquadramento do hero (`object-position` em `css/style.css`) e registre fonte e licença em `assets/img/CREDITS.md`.
Reveja o contraste do texto sobre o hero e a seção "Abordagem" com a foto real.
Mantenha o aviso de que as imagens são de demonstração enquanto a marca for fictícia.

## 3. Publicar
Qualquer hospedagem estática serve (Netlify, Vercel, GitHub Pages, Cloudflare Pages ou hospedagem comum):
envie a pasta inteira, com `index.html` na raiz.

## Textos a confirmar
- "Os detalhes da cobertura são definidos na conversa, de acordo com o casamento." (premissa)
- Mensagem de WhatsApp, legendas, textos alternativos e rodapé foram escritos para este projeto.
