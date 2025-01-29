# Resumo 1 - O que é Git?

Esse é o resumo sobre o que é o Git. Entenda sobre essa ferramenta e a sua função de modo intuitivo.
Para começar, precisamos entender o que é um VCS, ou sistema de versionamento de código.


## O que é um VCS? ⚙️

Um VCS - sistema de versionamento de código - tem por função verificar alterações em um sistema de arquivos, permitindo a integração e o compartilhamento das alterações com outros usuários do sistema.

### Tipos de VCS 📚

Existem dois tipos de VCS:
| | Centralizados | Distribuídos |
|--------|---------------|--------------|
| <div align="center">Descrição</div> |Baseados em um ponto central de falha, uma instância remota e centralizada do VCS. Caso essa instância seja perdida deverá ser substituida por uma nova cópia do código-fonte. Além disso, caso esteja indisponível, impedirá atualizações por parte dos desenvolvedores. | Baseados em instâncias com versões completas do código fonte, evitando as armadilhas de indisponibilidade de um VCS Centralizado. Caso a versão "original" seja perdida, basta que outra instância seja usada para liderar o desenvolvimento. |
| <div align="center">Exemplos</div> | <div align="center">![Static Badge](https://img.shields.io/badge/Subversion-81599F?style=for-the-badge&logo=subversion&logoColor=D9ECFF&logoSize=auto) ![Static Badge](https://img.shields.io/badge/Perforce-81599F?style=for-the-badge&logo=perforce&logoColor=D9ECFF&logoSize=auto)</div> | <div align="center">![Static Badge](https://img.shields.io/badge/Git-81599F?style=for-the-badge&logo=git&logoColor=D9ECFF&logoSize=auto) ![Static Badge](https://img.shields.io/badge/Mercurial-81599F?style=for-the-badge&logo=mercurial&logoColor=D9ECFF&logoSize=auto)</div> |
| <div align="center">Representação visual</div> | <div align="center"><img alt="VCS Centralizado" src="./../assets/imagens/centralized-vcs.png" width="100" height="100"></div> | <div align="center"><img alt="VCS Distribuido" src="./../assets/imagens/distributed-vcs.png" width="100" height="100"></div> |

### Por que eu preciso de VCS? 🤯

Os sistemas de versionamento são muito importantes para uma equipe de desenvolvimento, visto os seguintes pontos:

- Rastreabilidade: Quando, por quem e quais alterações foram feitas;
- Segurança: Permite a criação de backups externos do código, caso a versão originária apresente problemas;
- Agilidade e resolução de problemas: Ao longo da criação de um sistema, vários profissionais alteram o mesmo arquivo ao mesmo tempo. O VCS é essencial para que esse fluxo de trabalho paralelo aconteça, dando agilidade e permitindo a atualização adequada dos arquivos.


## O que é o Git? <img alt="VCS Distribuido" src="./../assets/imagens/git-logo.png" width="20" height="20">

O Git é essencialmente um sistema de versionamento de código distribuído, DVCS, open-source e gratuito.
Desse modo, é muito interessante usá-lo, visto que para ter ele em sua máquina basta usar o botão abaixo e seguir os passos da instalação:

[![Link do Git](https://img.shields.io/badge/Download-81599F?style=for-the-badge&logo=git&logoColor=D9ECFF&logoSize=auto&label=Git&labelColor=81599F&color=3CD4D9)](https://git-scm.com/downloads)

### Como o Git trata os arquivos? 🎲

O Git trata os dados do sistema de arquivos como um conjunto de imagens em miniatura. Sempre que há um `commit` uma nova imagem é capturada.
Para eficiência, o Git não armazena os arquivos novamente caso não tenham sido alterados. Ao invés disso, um link para o fluxo armazenado anteriormente é criado. Observe um esquemático da armazenamento do próprio Git:

<div align="center"><img alt="Armazenamento do Git]" src="./../assets/imagens/git-snapshot-schema.png" width="600"></div>

### Operações essenciais de um repositório Git. 🛠️
Em um repositório de arquivos baseado no git você pode executar diversas operações. Considero três delas muito importantes:
- Braching (```git checkout```): Permite que o desenvolvedor separe um "braço" de trabalho só para ele, possibilitando paralelismo a codificação;
- Merging: (```git push```, ```git pull``` e ```git merge```): Permite que a equipe combine as alterações em um único ponto do repositório, unindo-as;
- Rebasing (```git rebase```): Permite que você carregue uma sequência de mudanças de uma branch para outra. Pode ser útil para unir as branches, tal qual o merge. No entanto, pode ainda ser aplicado em casos específicos, como para possibilitar alterações de históricos - quando associado a outros comandos. 

A ilustração abaixo representa rapidamente o fluxo de trabalho de um repositório Git:

<div align="center"><img alt="Fluxo de trabalho de um repositório Git" src="./../assets/imagens/git-repository-graph.png" width="600"></div>

### Árvore de trabalho, Área de Preparação e Repositório Local 🖥️
O Git possui áreas de trabalho que são empregadas para garantir um fluxo adequado das alterações, mantendo a segurança e a validação das alterações antes que sejam de fato encaminhadas para o uso.
Existem três áreas, sendo elas:

| Nome | Árvore de trabalho (Working Tree) | Área de preparação (Staging Area) | Repositório Local (Local Repo) |
| Descrição |Pense na Working Tree como a sua área de trabalho no computador, onde você edita seus arquivos livremente. O Git observa essa área, mas não salva automaticamente suas mudanças. Se você modificar algo e não mandar para o Git (com comandos como ```git add``` e ```git commit```), suas alterações poderão ser perdidas. | A Staging Area funciona como um rascunho antes de salvar algo definitivamente. Quando você edita um arquivo, ele fica na Working Tree. Se quiser que o Git preste atenção nele, você usa ```git add```, e ele passa para a Staging Area. Apesar disso, se você editar o arquivo depois, o Git não verá as novas mudanças até que você as adicione novamente. 
Logo, a Staging Area ajuda a organizar as mudanças antes de salvá-las no histórico do Git com o ```git commit```. | O Repositório Local é como a memória do Git: ele guarda todo o histórico do seu projeto dentro do diretório ```.git```. Quando você usa o ```git commit```, é como tirar uma foto do estado atual dos arquivos. Isso cria um checkpoint, permitindo que você volte para esse ponto no futuro, se necessário.
Depois de um commit, a Staging Area fica limpa, pronta para novas mudanças. |

Observe a seguir uma representação simples da interação entre essas áreas: 

<div align="center"><img alt="Áreas de trabalho do Git" src="./../assets/imagens/git-areas-schema.png" width="400"></div>

## Referências para esse resumo 🔍
- [Software de controle de versão para equipes profissionais](https://bitbucket.org/product/br/version-control-software);
- [1.3 Começando - O Básico do Git](https://git-scm.com/book/pt-br/v2/Come%C3%A7ando-O-B%C3%A1sico-do-Git);
- [Git merge](https://www.atlassian.com/git/tutorials/using-branches/git-merge);
- [3.6 Branches no Git - Rebase](https://git-scm.com/book/pt-br/v2/Branches-no-Git-Rebase);
- [Versionamento de Código - Conceitos Básicos](https://www.dio.me/articles/versionamento-de-codigo-conceitos-basicos);
- [Git Gud: A árvore de trabalho, área de preparação e repositório local](https://medium.com/@lucasmaurer/git-gud-the-working-tree-staging-area-and-local-repo-a1f0f4822018).


## Autor ℹ️

- Feito com o 🫶🏻 por [@GabrielFAlmeida](https://github.com/GabrielFAlmeida)
- LinkedIn: [Gabriel França de Almeida](https://www.linkedin.com/in/gabriel-frnca/)
