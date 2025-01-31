# Resumo 5 - Trabalhando com branches 🔀

Esse é o resumo trata sobre como manipular as branches e usá-las para segmentar suas criações.


## Verificando as branches existentes ⏱️

Para listar quais branches estão disponíveis, basta usar o comando:

    git branch

## Adicionando um repositório remoto vinculado ao seu repositório local 🔛

Para vincular um repositório remoto ao seu local é simples:

    git remote add 

Por padrão o nome vinculado será ```origin```, ou seja, ```origin``` é o espaço remoto que será associado ao seu recurso local.
Além disso, você pode listar os repositórios ligados usando:

    git remote -v

## Operações comuns com branches 🔡

Usualmente, usamos as branches como divisões que permitem o pararelismo do trabalho em funcionalidades específicas. Portanto, podemos criar, deletar, mesclar e atualizar as branches - como atividades comuns.

Para criar uma nova branch e ir até ela, use:

    git checkout -b NOME_DA_BRANCH

Para deletar uma branch determinada, basta aplicar:


    git branch -d NOME_DA_BRANCH


Para atualizar sua branch principal ```main``` com o conteúdo da sua branch remota, presente em ```origin``` use:

    git fetch origin main

Para verificar quais são as diferenças entre duas branches, use:

    git diff NOME_DA_BRANCH_1 NOME_DA_BRANCH_2


Por fim, para mesclar duas branches, aplique:

    git merge NOME_DA_BRANCH_1 NOME_DA_BRANCH_2

## Referências para esse resumo 🔍

- [Comandos GIT - Comandos essenciais do Git para gerenciamento de branches](https://www.dio.me/articles/comandos-git-comandos-essenciais-do-git-para-gerenciamento-de-branches);
- [Git Fetch](https://git-scm.com/docs/git-fetch);
- [Git Merge](https://git-scm.com/docs/git-merge).

## Autor ℹ️

- Feito com o 🫶🏻 por [@GabrielFAlmeida](https://github.com/GabrielFAlmeida)
- LinkedIn: [Gabriel França de Almeida](https://www.linkedin.com/in/gabriel-frnca/)
