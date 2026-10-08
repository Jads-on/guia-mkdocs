# Como hospedar um site MkDocs no Github Pages?

&emsp;  Há dois tipos de sites GitHub Pages . Sites associados a uma conta de usuário ou organização e sites para um projeto específico.

## Tipo 1: Sites de projetos
&emsp; Exemplo: `github.com/usuario/meu-projeto`. Os arquivos compilados do site são enviados para uma branch específica chamada `gh-pages`.

&emsp; Passos no terminal (a partir da branch principal, geralmente `main`):

1. Certifique-se de que o projeto está versionado no Git 

    &emsp; Crie um repositório no Github e faça primeiro commit. Na pasta do seu projeto.
    !!! note "Como versionar o projeto"

        ```git init```

        ```git add .```

        ```git commit -m "Commit inicial da documentação"```

        ```git remote add origin https://github.com/seu-usuario/meu-projeto-mkdocs.git```

        ```git push -u origin main```

2. Execute o comando de deploy automático:

    ```
    mkdocs gh-deploy
    ```

&emsp; O que o comando faz nos bastidores: compila o site estático, cria/atualiza a branch `gh-pages` e envia (push) as alterações diretamente para o GitHub.

!!! warning "Avisos importantes para o Deploy"
    - Nunca edite arquivos manualmente na branch `gh-pages`, pois eles serão sobrescritos no próximo deploy.
    - Sempre teste o site localmente (`mkdocs serve`) antes de rodar o `gh-deploy`.

## Tipo 2: Sites de usuário ou organização
&emsp; Exemplo: `usuario.github.io`. Os arquivos do site precisam ser implantados na branch principal (`main`) de um repositório dedicado.

&emsp; Exemplo de comando apontando para a branch `main`:

    mkdocs gh-deploy --remote-branch main

