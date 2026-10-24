# Bento's Barbearia

Página de link na bio pro Instagram de uma barbearia. A ideia era ir além da lista de botões: além de levar o cliente a agendar, a página conta a história do dono, que começou do zero e abriu a própria barbearia.

<img src="Anexos/Bio%20Instagram%20-%20375px.png" alt="Página no celular" width="320">

Um `index.html` só, com HTML, CSS e JS puro, sem build. Está em [bio-instagram/](bio-instagram/).

## O que tem

- Botão de agendar em destaque. Se a barbearia não usa app de agenda, ele abre o WhatsApp com a mensagem pronta
- Selo de "Aberto agora" / "Fechado · abre terça às 9h", calculado no horário de Brasília mesmo se o celular estiver em outro fuso
- Horários num acordeão com o dia de hoje destacado
- Seção "Minha história" com foto, linha do tempo e uma frase do Bento, terminando com outro botão de agendar
- Lista de serviços e preços
- Dados estruturados `BarberShop` montados a partir do `CONFIG`, então os dados só são editados em um lugar

<img src="Anexos/Bio%20Instagram%20-%20hor%C3%A1rios.png" alt="Horários abertos" width="320">

Os dados da barbearia ainda estão como `[PLACEHOLDER]` enquanto eu não recebo as informações reais. Enquanto não tem logo nem foto, a página mostra um "B" e um quadro no lugar da foto.

## Rodando

```bash
cd bio-instagram
python3 -m http.server 8000
```

Pra testar o selo num horário específico: `?simular=sabado-21:30`.
