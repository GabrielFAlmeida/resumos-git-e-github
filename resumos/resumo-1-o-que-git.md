# Resumo 1 - O que é Git? 

Esse é o resumo sobre o que é o Git. Entenda sobre essa ferramenta e a sua função de modo intuitivo.
Para começar, precisamos entender o que é um VCS, ou sistema de versionamento de código.

## O que é um VCS? ⚙️
Um VCS - sistema de versionamento de código - tem por função verificar alterações em um sistema de arquivos, permitindo a integração e o compartilhamento das alterações com outros usuários do sistema.

### Tipos de VCS 📚
Existem dois tipos de VCS:
|        | Centralizados | Distribuídos |
|--------|---------------|--------------|
| Descrição |Baseados em um ponto central de falha, uma instância remota e centralizada do VCS. Caso essa instância seja perdida deverá ser substituida por uma nova cópia do código-fonte. Além disso, caso esteja indisponível, impedirá atualizações por parte dos desenvolvedores. | Baseados em instâncias com versões completas do código fonte, evitando as armadilhas de indisponibilidade de um VCS Centralizado. Caso a versão "original" seja perdida, basta que outra instância seja usada para liderar o desenvolvimento. |
| Exemplos | 
![Static Badge](https://img.shields.io/badge/Subversion-81599F?style=for-the-badge&logo=subversion&logoColor=D9ECFF&logoSize=auto) 
![Static Badge](https://img.shields.io/badge/Perforce-81599F?style=for-the-badge&logo=perforce&logoColor=D9ECFF&logoSize=auto)
| ![Static Badge](https://img.shields.io/badge/Git-81599F?style=for-the-badge&logo=git&logoColor=D9ECFF&logoSize=auto)
![Static Badge](https://img.shields.io/badge/Mercurial-81599F?style=for-the-badge&logo=mercurial&logoColor=D9ECFF&logoSize=auto) |
| Representação visual | <img alt="VCS Centralizado" src="./../assets/imagens/centralized-vcs.png" width="100" height="100"> | <img alt="VCS Distribuido" src="./../assets/imagens/distributed-vcs.png" width="100" height="100"> |

### Por que eu preciso de VCS? 🤯
Os sistemas de versionamento são muito importantes para uma equipe de desenvolvimento, visto os seguintes pontos:
- Rastreabilidade: Quando, por quem e quais alterações foram feitas;
- Segurança: Permite a criação de backups externos do código, caso a versão originária apresente problemas;
- Agilidade e resolução de problemas: Ao longo da criação de um sistema, vários profissionais alteram o mesmo arquivo ao mesmo tempo. O VCS é essencial para que esse fluxo de trabalho paralelo aconteça, dando agilidade e permitindo a atualização adequada dos arquivos.

## O que é o Git? 🔶
O Git é essencialmente um sistema de versionamento de código distribuído, DVCS, open-source e gratuito.
Desse modo, é muito interessante usá-lo, visto que para ter ele em sua máquina basta usar o botão abaixo e seguir os passos da instalação: 

[![Link do Git](https://img.shields.io/badge/Download-81599F?style=for-the-badge&logo=git&logoColor=D9ECFF&logoSize=auto&label=Git&labelColor=81599F&color=3CD4D9)](https://git-scm.com/downloads)

### Como o Git trata os arquivos? 🎲
O Git trata os dados do sistema de arquivos como um conjunto de imagens em miniatura. Sempre que há um ```commit``` uma nova imagem é capturada. 
Para eficiência o Git não armazena os arquivos novamente caso não tenham sido alterados. Ao invés disso, um link para o fluxo armazenado anteriormente é criado. Observe um esquemático da armazenamento do próprio Git: 

<img alt="Armazenamento do Git]" src="./../assets/imagens/git-snapshot-schema.png" width="200"> |
 
## Referências usadas para esse resumo 🔍
- [Versionamento de Código - Conceitos Básicos](https://www.dio.me/articles/versionamento-de-codigo-conceitos-basicos);
- [Git Gud: A árvore de trabalho, área de preparação e repositório local](https://medium.com/@lucasmaurer/git-gud-the-working-tree-staging-area-and-local-repo-a1f0f4822018);
- [Versionamento de Código, Git e GitHub - Guia Prático](https://www.dio.me/articles/versionamento-de-codigo-git-e-github-guia-pratico).
- [Software de controle de versão para equipes profissionais](https://bitbucket.org/product/br/version-control-software)

## Autor ℹ️

- Feito com o 🫶🏻 por [@GabrielFAlmeida](https://github.com/GabrielFAlmeida)
- LinkedIn: [Gabriel França de Almeida](https://www.linkedin.com/in/gabriel-frnca/)