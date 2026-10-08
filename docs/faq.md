# FAQ

# 1 - erro no comando pip 
## error: externally-managed-environment
&emsp; Este erro é comum em algumas distros linux, pois elas bloqueiam a instalação direta de pacotes Python via pip. A solução é instalar o Mkdocs em um ambiente isolado via pipx.

&emsp;  No terminal, digite:

    sudo apt update && sudo apt install pipx python3-full
  

&emsp;Após isso digite:
    
    pipx ensurepath
 
&emsp; Com isso, tanto o mkdocs quanto qualquer outra ferramenta instalada via `pipx install` ficam acessíveis globalmente, tudo sob administração do pipx .

&emsp; Para verificar a instalação:
    
    pipx --version
     
&emsp; Substitua os comando pip por pipx:
    
    pipx install mkdocs mkdocs-material
    
!!! note "Instalar temas e aplicativos na pasta isolada do pip"
    &emsp; Para instalar um tema ou aplicativo dentro da pasta isolada do mkdocs, substitua os comando `pip install` por `pipx inject`:

    &emsp; Exemplo: instalação do tema material:
        
        pipx inject mkdocs mkdocs-material
  
