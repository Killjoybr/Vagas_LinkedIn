# Vagas_LinkedIn

## Introdução
Quando você quer migrar de área ou simplesmente buscar por vagas na sua área, geralmente não sabemos como pesquisar ou precisamos filtrar algumas palavras. 

Este repositório possui 2 objetivos principais, ajudar pessoas empregadas ou desempregadas a encontrarem novas oportunidades e compilar algumas palavras chave, com ajuda da comunidade open-source, para facilitar na busca com base em vagas/ramo específicos.

## ToC Tabela de Conteúdo

- [Introdução](#introdução)
- [Exemplificação](#exemplificação)
- [Considerações](#considerações)

## Exemplificação

Modo comum: 
```txt
analista segurança da informação
```

Pesquisando desse modo eu encontrei vagas p/ analista de Bussines Intelligence, Analista de suporte técnico N2 e algumas vagas do meu interesse mas que já eram antigas e cheias de aplicantes.

Modo refinado:
```txt
"analista" AND ("segurança") NOT ("do Trabalho")
```
Só de adicionar aspas duplas na nossa pesquisa, sem os comandos SQL em seguida, já temos a pesquisa exata apenas com texto que contenha "analista" no resultado. 

Ao adicionar os comandos SQL AND e NOT filtramos ainda mais, o comando **AND** serve para **adicionar** a pesquisa principal "analista" o termo segurança, o comando **NOT** serve para remover qualquer resultado que contenha "do Trabalho"

O motivo principal dessa query é pesquisar por vagas de analista em segurança da informação, nos meus testes percebi que a remoção do termo "do Trabalho" me retornava majoritariamente vagas de Cibersegurança.

Note que pode ser utilizado também para vagas de estágio e com diferentes níveis de senioridade, seja adicionando o termo com a senioridade ou excluindo alguma senioridade.
```txt
"analista" AND ("segurança") NOT ("Senior")
```
```txt
"analista" AND ("segurança") AND ("Junior")
```

## Considerações

Fico disponível para contato para tirar quaisquer dúvidas sobre as pesquisas utilizando esse método, fico disponível em qualquer contato disponível no website [ruandavid.tech](https://ruandavid.tech)