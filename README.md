# Bitdevs interior do estado de São Paulo

Um site simples feito com `jekyll` para hospedar todos o links dos encontros
passados e futuros.

## Desenvolvimento

Você vai precisar do [Ruby & Jekyll](https://jekyllrb.com/docs/installation/)
para executar o site localmente. Uma vez configurado:

### clone o repositório

```bash
# sem ssh
git clone https://github.com/qlrd/bitdevsinteriorrr.git

# com ssh
git clone git@github.com:qlrd/bitdevsinteriorrr.git
```


### Vá até o diretório

```bash
cd bitdevsinteriorrr
```

### Instale as dependências

```bash
bundle install
```

### Execute

```bash
jekyll serve
```

E abra `http://localhost:4000` no seu navegador.

## Crie um post

Para fazer um novo post, crie um novo arquivo em `_posts/` com o título na forma
`YYYY-MM-DD-title-goes-here`. No cabeçalho deste arquivo você irá fornecer as
seguintes informações:

```md
---
layout: post # Always post
type: socratic # or whitepaper for a whitepaper series
title: "Name of the Post"
meetup: https://www.meetup.com/bitdevsinteriorrr/events/[event id here]/
---
```

Depois disso, é um simples arquivo `markdown`. O site irá auto-gerar o resto.

## Mudando configurações

Todas as configurações estão ou contidas em `_config.yml` 
`_data/settings.yml`. Alguns dados estão duplicados entre os dois de forma
que o Jekyll injeta variáveis. Tenha certeza de fazer update em ambos.

## Atribuições

Obrigado ao [LeNPaul](https://github.com/LeNPaul/jekyll-starter-kit) pelo kit
de inicialização do Jekyll, do qual este foi forkado.
