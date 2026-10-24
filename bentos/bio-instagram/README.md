# Link na bio

A página toda é o `index.html` e a pasta `assets/`.

## Configuração

Os dados ficam no `CONFIG`, no `<script>` perto do fim do arquivo:

| Campo | |
|---|---|
| `slogan` | frase embaixo do nome |
| `whatsapp` | DDD + número, só dígitos |
| `mensagemWhatsapp` | texto que já vem escrito no botão de WhatsApp |
| `mensagemAgendamento` | texto usado no botão de agendar quando não tem `linkAgendamento` |
| `linkAgendamento` | link do app de agenda (Booksy, Trinks...). Vazio = agenda pelo WhatsApp |
| `linkMapa`, `linkInstagram`, `endereco` | |
| `horarios` | `'HH:MM-HH:MM'` por dia, `null` = fechado |
| `servicos` | lista de `{ nome, preco }`. Vazia esconde a seção |

O texto da história fica direto no HTML, na seção "Minha história". O console avisa o que ainda está com `[...]`.

## Imagens

Em `assets/`:

- `logo.png` e `logo.webp`, quadrados
- `bento.jpg`, foto em pé (uns 800x1000)

Se não existirem, a página mostra um "B" no lugar do logo e um quadro no lugar da foto. O `og-image.jpg`, o favicon e o apple-touch-icon ainda são provisórios.

Depois de publicar, trocar `[URL_DO_SITE]` nas tags `og:` do `<head>` pra prévia do link funcionar no WhatsApp.
