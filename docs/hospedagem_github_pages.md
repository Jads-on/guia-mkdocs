# Hospedagem e portabilidade
&emsp; O MkDocs compila o conteúdo em páginas HTML/CSS/JS estáticas. Pode ser hospedado gratuitamente no GitHub Pages, GitLab Pages, Amazon S3, Netlify, Vercel ou em qualquer servidor web convencional.

#GitHub Pages 
&emsp; GitHub Pages é um serviço de hospedagem de sites estáticos que obtém arquivos HTML, CSS e JavaScript diretamente de um repositório no GitHub, opcionalmente os submete a um processo de build e publica um site.

&emsp; Os sites hospedados no GitHub Pages estão sujeitos aos seguintes limites de uso:

- Você só pode criar um site de usuário ou organização para cada conta GitHub;
- Os repositórios de origem e os sites publicados têm um limite recomendado de 1 GB;
- Os os sites têm um limite de largura de banda flexível de 100 GB por mês.
- Os os sites têm um limite flexível de 10 builds por hora. Esse limite não se aplicará se você criar e publicar seu site com um fluxo de trabalho personalizado GitHub Actions .
- Para fornecer qualidade de serviço consistente para todos os GitHub Pages sites, os limites de taxa podem ser aplicados. Esses limites de taxa não se destinam a interferir nos usos legítimos de GitHub Pages. Se a sua solicitação disparar a limitação de taxa, você receberá uma resposta apropriada com um código de status HTTP de 429, juntamente com um corpo HTML informativo.

&emsp; Se seu site exceder essas cotas de uso, talvez não possamos atender seu site ou você poderá receber um email Suporte do GitHub sugerindo estratégias para reduzir o impacto do seu site nos servidores do GitHub.

!!! note "Requisitos"
    É obrigatório ter o git instalado. O **Git** é um sistema de controle de versão essencial para publicar e atualizar sua documentação automaticamente no **GitHub Pages** utilizando o comando `mkdocs gh-deploy`. Caso não tenha instale pelo comando: 
    
    - Linux:
    
    ```sudo apt update``` 
    
    ```sudo apt install git -y```
    
    - Windows:
    
    ```winget install --id Git.Git -e --source winget```
    
    Verificar se instalou corretamente:
    
    ```git --version```
    

