## Pré-requisitos de instalação
&emsp; Requisitos do Sistema:

1. Python (versão 3.8 ou superior)
2. pip (gerenciador de pacotes oficial do Python)
3. Git (necessário para controle de versão e para realizar o deploy no GitHub Pages)

&emsp; Verificando as versões instaladas (Terminal / Prompt de Comando):

    python --version (Windows)
    python3 --version (Linux)
    pip --version
    git --version

&emsp; Atualizando o pip para a versão mais recente:

    python -m pip install --upgrade pip

&emsp; Instalando o MkDocs e o Tema Material:

    pip install mkdocs mkdocs-material

&emsp; Verificando a instalação do MkDocs:

    mkdocs --version

!!! note "Observação para usuários do Windows"
    Caso os comandos diretos apresentem erro de caminho (PATH), utilize o prefixo `python -m`:
    
    &emsp; Instalando o MkDocs e o Tema Material:

        python -m pip install mkdocs mkdocs-material

    &emsp; Verificando a instalação do MkDocs:

        python -m mkdocs --version
    

### O que é o "mkdocs-material"?
&emsp; É o tema visual mais popular e utilizado no ecossistema MkDocs. Adiciona recursos modernos como:

- Design responsivo
- Modo escuro/claro
- Pesquisa avançada
- Suporte a abas de código
- Avisos em caixas (admonitions)
- Ícones customizados

