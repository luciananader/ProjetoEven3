
# Chat IA Mentora de TCC

Este é o frontend de um projeto de chatbot educacional construído em HTML, CSS e JavaScript puro. Ele se conecta com um backend em FastAPI para simular uma mentora de TCC.

## Estrutura

- `index.html` — Página principal do chat.
- `style.css` — Estilo do chat.
- `script.js` — Lógica de envio e exibição de mensagens.
- `config.js` — Define a URL do backend.

## Funcionalidades

- Interface de chat para conversa com a IA.
- Envia mensagens para o backend via API.
- Exibe respostas da IA.
- Reseta o campo de input após o envio.
- Usa `Enter` para enviar a mensagem.

## Como Rodar Localmente

1. Clone o repositório:
   ```bash
   git clone https://github.com/seu-usuario/seu-repo-frontend.git
   cd seu-repo-frontend
   ```

2. Edite o arquivo `config.js` para apontar para sua API:
   ```js
   const API_BASE_URL = "https://seu-backend-na-render.onrender.com";
   ```

3. Abra o `index.html` no navegador.

> Você pode usar a extensão do VSCode “Live Server” para recarregar automaticamente.

## Deploy com GitHub Pages

Se quiser hospedar este frontend com GitHub Pages:

1. Vá em `Settings > Pages`.
2. Escolha a branch `main` e a pasta `/root`.
3. Salve e acesse a URL gerada (ex: https://seu-usuario.github.io/seu-repo-frontend/).

## Integração com o Backend

Certifique-se de que seu backend está rodando e acessível publicamente, por exemplo via Render: `https://seu-backend.onrender.com`.

O frontend envia requisições POST para:
```
POST /chat
Content-Type: application/json

{
  "message": "sua mensagem"
}
```

