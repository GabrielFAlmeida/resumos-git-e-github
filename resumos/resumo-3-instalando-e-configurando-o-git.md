# Resumo 3 - Como instalar e configurar o Git? ⬇️

Esse é o resumo sobre como fazer o Git funcionar em seu computador, ou seja, como instalar e fazer a configuração desse sistema.


## Instalando o Git 

Abaixo como instalar o recurso nos principais sistemas operacionais.

### Instalando no Windows <img alt="GitHub" src="./../assets/imagens/windows.png" width="20" height="20">

- Acesse o site do Git e faça o download do instalador:

[![Git](https://img.shields.io/badge/Download-81599F?style=for-the-badge&logo=git&logoColor=%23D9ECFF&logoSize=auto&label=Git&labelColor=81599F&color=3CD4D9)](https://git-scm.com/downloads/win)

- Execute o instalador;
- Aceite a licença;
- Selecione as preferências que tiver durante a instalação;
- Finalize ao clicar em "Instalar/Install".

### Instalando no Linux <img alt="GitHub" src="./../assets/imagens/linux.png" width="20" height="20">

- Acesse o site do Git e confira a documentação:

[![Git](https://img.shields.io/badge/Documentação-81599F?style=for-the-badge&logo=git&logoColor=%23D9ECFF&logoSize=auto&label=Git&labelColor=81599F&color=3CD4D9)](https://git-scm.com/downloads/linux)

- Para a última versão estável da sua release do Debian/Ubuntu

    ```
    # apt-get install git
    ```

- Para o Ubuntu, esse processo fornece a versão estável mais recente do Git:
    ```
    # add-apt-repository ppa:git-core/ppa
    ```

    ```
    # apt update; apt install git
    ```

- Para outras distribuições do Linux siga a documentação indicada acima.

### Instalando no MacOS <img alt="GitHub" src="./../assets/imagens/apple.png" width="20" height="20">

- Caso não tenha o HomeBrew ou o MacPorts, instale um desses:

[![Homebrew](https://img.shields.io/badge/Download-81599F?style=for-the-badge&logo=homebrew&logoColor=%23D9ECFF&logoSize=auto&label=Homebrew&labelColor=81599F&color=3CD4D9
)](https://brew.sh/)


[![MacPorts](https://img.shields.io/badge/Download-81599F?style=for-the-badge&logoColor=%23D9ECFF&logoSize=auto&label=MacPorts&labelColor=81599F&color=3CD4D9)](https://www.macports.org/install.php)

- Usando o Homebrew, basta executar o comando

    ```
    $brew install git
    ```

- Para o MacPorts, execute esse código:

    ```
    sudo port install git
    ```

## Configurando o Git 🔑

Nessa parte do conteúdo você acessará como configurar partes essenciais do Git.

Para iniciar, você pode listar as configurações do seu Git com o seguinte comando:
Além disso, é importante evidenciar que existem três tipos de configurações no Git, sendo elas:
- --global: configurações globais, relacionadas ao seu usuário;
- -- system: configurações fixadas ao sistema apenas;
- --local: configurações do repositório em específico.

### Configurando seu usuário e o nome da branch padrão:
Para configurar globalmente o seu usuário, você usará os dois comandos a seguir:
Para configurar o nome da branch padrão dos repositórios, globalmente, você deve usar o código a seguir:
Atualmente, usamos o nome ```main``` para nossas branches padrão. Em alguns repositórios mais antigos você também pode vê-las com o nome ```master```.

## Referências para esse resumo 🔍

- [Downloads](https://git-scm.com/downloads).

## Autor ℹ️

- Feito com o 🫶🏻 por [@GabrielFAlmeida](https://github.com/GabrielFAlmeida)
- LinkedIn: [Gabriel França de Almeida](https://www.linkedin.com/in/gabriel-frnca/)
