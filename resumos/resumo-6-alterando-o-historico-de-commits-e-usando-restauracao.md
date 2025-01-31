# Resumo 6 - Alterando o histórico de commits e usando restauração? ↩️

Esse é o resumo sobre como verificar o que já aconteceu no seu repo e editar as informações, caso seja

## Como verificar o que foi commitado? ⁉️

Para verificarmos o que foi commitado no seu repo podemos usar:

    git log

Vale lembrar que pastas vazias não são consideradas para seus commits. A não ser que você use arquivos ```.gitkeep```.
Caso você mude o histórico de commits, você ainda pode validar todas as operações feitas usando o:

    git reflog

### .Gitkeep e .gitignore ❌✅

Arquivos ```.gitkeep``` são usados para especificar uma pasta que deve ser mantida, ainda que esteja vazia. É importante adicionar o arquivo a estrutura que deve ser mantida. 

Além disso, há o arquivo ```.gitignore```, adicionado ao projeto como um todo. Esse arquivo é ainda mais comum que o anterior. Para fins de demonstração, esse repositório possui os dois tipos em questão.

## Resetando commits ⏲️

É possível fazer um reset de informações de um commit, com o comando:

    git reset

É importante sinalizar que podemos fazer a adicação de um parâmetro com o local do arquivo, isso permite a remoção de um conteúdo especifico.
Além disso, existem três tipos de operações de reset:
- --soft: desfaz os commits posteriores ao escolhido e deixa os arquivos removidos na área de preparação;
- --mixed: defaz os commits feitos após o escolhido, mas os deixam na árvore de trabalho;
- --hard: defaz permanentemente os commits posteriores ao escolhido, deletando os arquivos.

## Alterando comentários de commits

Você pode corrigir ou alterar uma mensagem do último commit com base no seguinte comando:

    git commit --amend -m "NOVA_MENSAGEM"

Para alterar mensagens mais antigas, será necessário usar o ```git rebase``` antes do comando de edição.

## Restaurando um arquivo
É possível restaurar a última versão salva de um arquivo através do comando:

    git restore

Ou ainda, remover arquivos da sua área de preparação por meio da adição do parâmetro ```--staged``` ao final do ```git restore```.

## Referências para esse resumo 🔍

- [Git Log](https://git-scm.com/docs/git-log);
- [Git Reflog](https://git-scm.com/docs/git-reflog);
- [7.6 Git Tools - Rewriting History](https://git-scm.com/book/en/v2/Git-Tools-Rewriting-History);
- [Git Reset](https://git-scm.com/docs/git-reset);
- [Git Restore](https://git-scm.com/docs/git-restore).

## Autor ℹ️

- Feito com o 🫶🏻 por [@GabrielFAlmeida](https://github.com/GabrielFAlmeida)
- LinkedIn: [Gabriel França de Almeida](https://www.linkedin.com/in/gabriel-frnca/)
