# JS em 3 Níveis

Três jogos em **JavaScript puro** (sem frameworks), organizados em ordem crescente de dificuldade para treinar lógica de programação.

🔗 Abra `index.html` no navegador ou publique com o GitHub Pages (veja abaixo).

## Os três níveis

| Nível | Jogo | Conceito principal em JS | Elemento HTML usado |
|---|---|---|---|
| 1 | Adivinhe o Número | Condicionais (`if/else`) e números aleatórios (`Math.random`) | `<input>` e `<button>` |
| 2 | Jogo da Velha | Array de estado e eventos de clique | Grade com `<div>`/CSS Grid |
| 3 | Cobrinha | API Canvas, `keydown` e loop com `setInterval` | `<canvas>` |

## Estrutura do projeto

```
jogos-js/
├── index.html      # menu com os 3 níveis
├── nivel1.html      # Adivinhe o Número
├── nivel2.html      # Jogo da Velha
├── nivel3.html      # Cobrinha
├── css/
│   └── style.css    # estilo compartilhado pelas 4 páginas
└── js/
    ├── nivel1.js
    ├── nivel2.js
    └── nivel3.js
```

Nenhuma dependência externa além de uma fonte do Google Fonts carregada via `@import` no CSS — não há build step, `npm install` ou framework algum.

## Rodando localmente

Basta abrir `index.html` diretamente no navegador. Se preferir servir por HTTP (recomendado para o Canvas funcionar sem restrições de alguns navegadores):

```bash
python3 -m http.server 8000
# depois acesse http://localhost:8000
```

## Publicando no GitHub Pages

1. Crie um repositório no GitHub e suba este código (veja os comandos no final da entrega).
2. No repositório, vá em **Settings → Pages**.
3. Em "Source", selecione a branch `main` e a pasta `/ (root)`.
4. Salve — o GitHub gera uma URL do tipo `https://SEU-USUARIO.github.io/NOME-DO-REPO/`.

## Controles

- **Nível 1**: digite um número e clique em "Chutar".
- **Nível 2**: clique nas casas do tabuleiro (alterna X e O).
- **Nível 3**: setas do teclado (ou WASD); no celular, use os botões na tela.
