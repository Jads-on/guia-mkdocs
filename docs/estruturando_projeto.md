## Criando e estruturando um projeto
&emsp; Criando um novo projeto via linha de comando:

    mkdocs new meu-projeto
    cd meu-projeto

&emsp; Estrutura de arquivos gerada:

```
meu-projeto/
├── mkdocs.yml    <-- Arquivo de configuração principal (YAML)
└── docs/         <-- Pasta com os arquivos de conteúdo (Markdown)
    └── index.md  <-- Página inicial da documentação
```

## Adicionando páginas e configurando a navegação
&emsp; Para criar novos arquivos de conteúdo, basta adicionar arquivos com extensão `.md` dentro da pasta `docs/`. Exemplo: `docs/about.md` (Página Sobre).

&emsp; Configurando o arquivo `mkdocs.yml` para ativar o tema Material e definir o menu de navegação (`nav`):

```yaml
site_name: Documentação do Meu Projeto
site_description: Guia do usuário e referências.
site_author: Seu Nome

theme:
  name: material

nav:
  - Início: index.md
  - Sobre: about.md
```

&emsp; Recursos gerados automaticamente pelo MkDocs:

1. Menu de Navegação: barra lateral/superior organizada de acordo com a chave `nav`
2. Botões de Navegação Sequencial: links para "Anterior" (Previous) e "Próximo" (Next)
3. Busca Interna Automatizada: campo de pesquisa funcional que indexa todo o texto do site sem necessidade de configuração adicionals

&emsp; Iniciando o servidor de desenvolvimento local:

    mkdocs serve

&emsp; Saída esperada no terminal:

```
INFO    -  Building documentation...
INFO    -  Cleaning site directory
INFO    -  Documentation built in 0.22 seconds
INFO    -  [15:50:43] Watching paths for changes: 'docs', 'mkdocs.yml'
INFO    -  [15:50:43] Serving on http://127.0.0.1:8000/
```

&emsp; Acessando o site localmente, basta abrir no navegador o endereço `http://127.0.0.1:8000/`. Qualquer alteração salva nos arquivos da pasta `docs/` ou no `mkdocs.yml` recarregará a página automaticamente no navegador (Live Reload).


