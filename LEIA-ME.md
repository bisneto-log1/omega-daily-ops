# OMEGA // Operações do Dia — Guia de Instalação

Este é um PWA (Progressive Web App): um app real, instalável, que funciona
100% offline depois de instalado. Os dados ficam salvos no `localStorage`
do seu navegador/dispositivo — nada vai pra nuvem, nada depende de internet
depois do primeiro carregamento.

## Arquivos
- `index.html` — o app
- `manifest.json` — identidade do app (nome, ícone, cor)
- `service-worker.js` — cache offline
- `icon-192.png`, `icon-512.png`, `icon-180.png`, `icon-32.png` — ícones

## Como colocar no ar (grátis, 5 minutos) — GitHub Pages

Você já tem noção de HTML pelo IFRN, então isso vai ser tranquilo:

1. Crie uma conta em github.com (se ainda não tiver).
2. Crie um repositório novo, público, nome sugerido: `omega-ops`.
3. Faça upload de todos os arquivos desta pasta pra raiz do repositório
   (botão "Add file" → "Upload files" no site do GitHub, sem precisar de terminal).
4. Vá em **Settings → Pages** → em "Source" selecione a branch `main` e
   a pasta `/ (root)` → Save.
5. Espere ~1 minuto. Seu app estará em:
   `https://SEU-USUARIO.github.io/omega-ops/`

## Como instalar no celular

**Android (Chrome):**
Abra o link acima → menu (⋮) → "Instalar app" ou "Adicionar à tela inicial".
Vai aparecer um banner amarelo no próprio app oferecendo instalar também.

**iPhone (Safari):**
Abra o link acima → ícone de compartilhar (□↑) → "Adicionar à Tela de Início".

Depois de instalado, o ícone Ômega aparece na tela inicial, abre em tela
cheia sem barra de navegador, e funciona sem internet.

## Nota sobre "sem servidor"

Dá pra abrir o `index.html` direto do celular (por email, Drive, etc.) e
ele funciona — mas o comportamento de "instalar como app de verdade" com
ícone e modo offline pleno só é garantido com hospedagem via HTTPS, por
regra dos próprios navegadores (Safari em especial é rígido nisso). Por
isso o GitHub Pages é o caminho recomendado — é grátis e permanente.
