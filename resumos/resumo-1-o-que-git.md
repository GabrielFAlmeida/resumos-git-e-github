# Resumo 1 - O que é Git? 

Esse é o resumo sobre o que é o Git. Para definirmos basicamente o que ele faz, vamos falar sobre VCS, ou sistemas de versionamento de código.

## O que é um VCS? 🔨
Um VCS tem por função verificar alterações em um sistema de arquivos, permitindo a integração e o compartilhamento das alterações com outros usuários do sistema.

Existem dois tipos de VCS:
|        | Centralizados | Distribuídos |
|--------|---------------|--------------|
| Como funcionam? |Baseados em um ponto central de falha, uma instância remota e centralizada do VCS. Caso essa instância seja perdida deverá ser substituida por uma nova cópia do código-fonte. Além disso, caso esteja indisponível, impedirá atualizações por parte dos desenvolvedores. | Baseados em instâncias com versoes completas do código fonte, evitando as armadilhas de indisponibilidade de um VCS Centralizado. Caso a versão "original" seja perdida, basta que outra instância seja usada para liderar o desenvolvimento. |
| Exemplos | SVN, CVS e Perforce | GIT, Mercurial e Bazaar |
| Representação visual | ![VCS Centralizado](./../imagens/centralized-vcs.png) | ![VCS Distribuído](./../imagens/distributed-vcs.png) |

## Por que eu preciso de VCS? 🤯
Os sistemas de versionamento são muito importantes para uma equipe de desenvolvimento, visto os seguintes pontos:
- Rastreabilidade: Quando, por quem e quais alterações foram feitas;
- Segurança: Permite a criação de backups externos do código, caso a versão originária apresente problemas;
- Agilidade e resolução de problemas: Ao longo da criação de um sistema, vários profissionais alteram o mesmo arquivo ao mesmo tempo. O VCS é essencial para que esse fluxo de trabalho paralelo aconteça, dando agilidade e permitindo a atualização adequada dos arquivos.
 
## Referências usadas para esse resumo 🔍
- [Versionamento de Código - Conceitos Básicos](https://www.dio.me/articles/versionamento-de-codigo-conceitos-basicos);
- [Git Gud: A árvore de trabalho, área de preparação e repositório local](https://medium.com/@lucasmaurer/git-gud-the-working-tree-staging-area-and-local-repo-a1f0f4822018);
- [Versionamento de Código, Git e GitHub - Guia Prático](https://www.dio.me/articles/versionamento-de-codigo-git-e-github-guia-pratico).
- [Versionamento de Código, Git e GitHub - Guia Prático](https://www.dio.me/articles/versionamento-de-codigo-git-e-github-guia-pratico).
- [Software de controle de versão para equipes profissionais](https://bitbucket.org/product/br/version-control-software)

## Autor

- GitHub: [@GabrielFAlmeida](https://github.com/GabrielFAlmeida)
- LinkedIn: [Gabriel França de Almeida](https://www.linkedin.com/in/gabriel-frnca/)