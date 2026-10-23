# app-correicao – página de instalação do app Correição TRT12

Este repositório **não contém o app**. Ele guarda apenas a página que permite instalar o app da Corregedoria Regional do TRT12 na tela inicial do celular, com ícone e nome próprios.

**Link para instalar:** https://geison99.github.io/app-correicao/

## Para que serve

O app da Correição é um web app do Google Apps Script. O Apps Script não permite definir o ícone que o Android e o iPhone usam na tela inicial, e o atalho salvo direto do link do app fica com o ícone do Google.

Esta página resolve isso:

- **Aberta no navegador:** mostra as instruções de instalação para Android (Chrome) e iPhone (Safari).
- **Aberta pelo ícone da tela inicial:** redireciona na hora para o app.

O acesso ao app continua exigindo login com uma conta **@trt12.jus.br** autorizada pela Corregedoria. Esta página não contém dados das correições.

## Arquivos

| Arquivo | Função |
|---|---|
| `index.html` | Página de instruções. Também faz o redirecionamento: o link do app está na variável `APP` |
| `manifest.webmanifest` | Nome, cores e ícones do app para o Android |
| `apple-touch-icon.png` | Ícone do iPhone (180 px) |
| `icon-192.png`, `icon-512.png` | Ícones do Android |
| `favicon-32.png` | Ícone da aba do navegador, também usado pelo próprio app |

## Projeto principal

O código do app (Google Apps Script) fica no repositório **privado** `geison99/AppCorreicao`. Este repositório entra nele como submódulo, na pasta `lancador/`.

A página é publicada pelo GitHub Pages a partir da branch `main`. Cada push atualiza o site em cerca de um minuto.
