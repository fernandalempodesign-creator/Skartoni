# Skartoni — Cenografia sustentável e acessível

Site interativo de divulgação da **Skartoni**, empresa fictícia de cenografia em papelão criada como projeto acadêmico. Apresenta a empresa, o portfólio do primeiro trabalho (o cenário de *"Cisne Somos"*, com o elenco do Centro Paralímpico Brasileiro, direção de Stella Tobar), os serviços e o custo do material.

## Arquivos

- `skartoni.html` — o site inteiro em um único arquivo. Imagens, logo, texturas e a fonte dos títulos estão embutidos nele.
- `README.md` — este arquivo.

Para publicar na raiz de um endereço, renomeie `skartoni.html` para `index.html`.

## O que o site tem

- **Início:** logo e frase da empresa sobre o fundo de papelão.
- **Sobre:** o que a Skartoni faz, em quatro cards (Papelão, Desenho Universal, Peças que o ator move, Para quem).
- **Palco:** as seis peças do cenário (ovo, televisão, microfones, pódio, volante e ondas). Clique em uma peça para ver detalhes, use anterior/próxima, clique na imagem para ampliar.
  - **Audiodescrição:** botão que mostra a descrição da peça em texto.
  - **Ouvir:** lê a descrição em voz alta, usando a voz do navegador em pt-BR. Depende do suporte do navegador.
- **Serviços:** kit cenográfico, projeto cenográfico, oficina de papelão e peça avulsa, com os preços "a partir de".
- **Custo:** R$ 281,12 de material, com barras por categoria.
- **Quem somos:** as cinco sócias.

O site abre no modo noturno. O botão ◐ do menu alterna para o claro, mas a página volta ao noturno ao recarregar.

## Como publicar

Qualquer hospedagem de site estático serve:

- **Netlify Drop:** arraste o `index.html` em app.netlify.com/drop.
- **GitHub Pages:** envie o `index.html` para um repositório e ative o Pages nas configurações.
- **Vercel:** crie um projeto e envie o `index.html`.

## Como editar

Abra o arquivo em um editor de texto. As partes mais úteis:

- **Textos das seções:** estão no HTML, entre as tags `<section>`.
- **Peças do palco:** na lista `P`, dentro do `<script>`. Cada peça tem nome (`n`), descrição (`d`) e audiodescrição (`a`).
- **Gastos por categoria:** na lista `B`, também dentro do `<script>`.
- **Cores e tema:** variáveis no começo do `<style>` (`--bg`, `--ink`, `--head`, `--brown`). O tema noturno está na regra `:root[data-theme="dark"]`. Para abrir no claro, troque `data-theme="dark"` por `data-theme="light"` na tag `<html>` e `content="dark"` por `content="light"` na tag `<meta name="color-scheme">`.

## Tipografia

- **Títulos:** Oxidisaster, embutida no arquivo.
- **Textos:** Alegreya, carregada pelo Google Fonts (precisa de internet).

A Oxidisaster não tem acentos nas letras maiúsculas. Os glifos acentuados (Á, É, Í, Ó, Ú, Ã, Õ, Ç etc.) foram montados juntando a letra com o acento da própria fonte, então o desenho deles é aproximado.

## Licença da fonte

A Oxidisaster é gratuita apenas para uso pessoal e sem fins lucrativos. Existe licença comercial, que deve ser pedida ao autor (informações na página da fonte no FontSpace). Se a Skartoni virar uma empresa real, a licença comercial será necessária.

## Créditos

Fernanda Lempo, Juliana Lopez, Mariana de Souza, Lívia D'Angelo e Vivien Rodrigues.

Skartoni é uma empresa fictícia criada como projeto acadêmico.
