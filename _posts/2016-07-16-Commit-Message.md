---
layout: post
title:  "Série Contribuindo: uma boa mensagem de _commit_"
date:   2016-07-16 23:06:58
categories: github guide contributing
---

# Série: Contribuindo

## Faça uma boa mensagem de commit

* Se é um pequeno _commit_ tudo bem abreviar a mensagem com apenas um título com o comando `git commit -am "uma descricao do que este commit faz em ate 50 caracteres"`
* Mas se é um _commit_ que vai influenciar muito o código de outros _ramos_ ou que vai ser usado para _pull request_ então é importante escrever uma boa mensagem. Neste caso, **não** use o comando abreviado. Use os comandos:
    - `git add arquivo` : se necessário adicionar algum arquivo
    - `git commit` : sem abreviação e sem mensagem. Este comando vai abrir o _vi_ (ou seu editor preferido) para você digitar uma mensagem de _commit_ maior.
        * Na primeira linha, escreva um título do _commit_ com até 50 caracteres, como você já está acostumado.
        * Pule uma linha.
        * Da terceira linha para baixo, descreva com mais detalhes tudo o que você fez, o que este _commit_ inclui, o que muda, qual funcionalidade é acrescentada ou _bug_ é resolvido.
        * Saia com `:x` (no _vi_) para salvar e fazer o _commit_
        * Saia com `:q!` (no _vi_) para abortar a edição e **não** fazer o _commit_
        * Linhas iniciadas com \# são ignoradas pelo _git_ como sendo comentários e não são escritas no _commit_.
* Exemplo de uma boa mensagem de _commit_:

```
Faz um exemplo para demonstrar a clareza do commit

Sem este commit a explicação sobre mensagens de commit ficaria 
falha, sem um exemplo concreto. Este é um problema, porque assim 
fica apenas na imaginação o que seria um bom commit.Este commit 
corrige este problema ao fazer aqui um exemplo concreto e imperativo.

A primeira linha é um título imperativo descritivo do essencial. 
Os dois parágrafos seguintes, o de cima e este, são explicações mais 
aprofundadas. É importante descrever:

(1) _o que ocorria_ antes do commit, 
(2) _qual_ é o problema que este commit resolve, 
(3) _porque_ este comportamento é problemático, e 
(4) _como_ este commit corrige este problema.

Também é possível usar enumerações para clarificar algumas mudanças 
em pontos específicos, como:

* mudafunc() : agora não retorna mais void e sim o código do cliente
* funcoutra() : criada para cumprir outra finalidade que faltava
* divideaqui() : criada para cumprir uma finalidade tal e tal que 
antes estava sendo feita na função mudafunc() de modo a ficar mais 
clara a divisão do que cada função faz.
```

Lembre que a primeira linha é importante para ver o _log_ e acompanhar a evolução do programa.

* Referência: [A Note About Git Commit Messages](http://tbaggery.com/2008/04/19/a-note-about-git-commit-messages.html)

