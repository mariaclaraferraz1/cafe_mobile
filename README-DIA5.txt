# Café Mobile — Dia 5

## O que foi implementado
- PWA: `manifest.json`, ícones e registro do Service Worker.
- Cache dos arquivos essenciais para abertura offline (`sw.js`).
- Botão de instalação compatível com navegadores que oferecem `beforeinstallprompt`.
- Compartilhamento do resumo do pedido pela Web Share API, com cópia como alternativa.
- Compartilhamento das fotos da galeria como arquivo.
- Botão de compartilhar desativado quando o pedido está vazio.
- Ícone maskable incluído também na lista de arquivos do cache.

## Como testar
1. Publique a pasta `dia5` no GitHub Pages (Settings → Pages → Deploy from a branch).
2. Abra o endereço HTTPS publicado.
3. No computador, confira DevTools → Application → Manifest, Service Workers e Cache Storage.
4. No celular, abra o mesmo endereço HTTPS. No Android, use Instalar quando aparecer; no iPhone, Compartilhar → Adicionar à Tela de Início.
5. Adicione um produto e teste Compartilhar pedido.
6. Na aba Meu Café, tire/adicione uma foto e teste o botão 📤.
7. Depois de abrir o app conectado, ative o modo avião e reabra pelo ícone para testar o cache offline.

## Provas que devem ser anexadas na atividade
As capturas precisam ser feitas no seu próprio navegador, conta do GitHub e celular — não é possível produzir imagens verdadeiras dessas telas sem acessar esses dispositivos/contas.

- `01-app-navegador.png`: Café Mobile aberto no navegador.
- `02-github-arquivos.png`: repositório mostrando os arquivos do Dia 5 (`manifest.json`, `sw.js`, `js/pwa.js` e pasta `icons`).
- `03-github-pages.png`: Settings → Pages mostrando a publicação e o endereço HTTPS.
- `04-celular-app.png`: app aberto no celular ou ícone na tela inicial.
- `05-celular-compartilhar.png`: janela nativa de compartilhamento do pedido ou de uma foto.
- `06-offline.png` (opcional): app funcionando em modo avião.

## Validação técnica realizada
- Todos os arquivos JavaScript passaram por `node --check`.
- `manifest.json` foi validado como JSON.
- Não foram simuladas capturas de tela do GitHub ou do celular.
