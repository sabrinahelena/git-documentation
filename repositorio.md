# Iniciando repositório

- ## Criar repositório novo no github já possuindo a pasta que quer subir.
    - ### Clique em criar repositório e não selecione nada. 
    - ### Na segunda instrução do github, siga os passos (...or push an existing repository from the command line) IMPORTANTE: DAR GIT INIT ANTES!
    ```
    git init
    git remote add origin https://github.com/sabrinahelena/git-documentation.git 
    git branch -M main
    git push -u origin main
    ```
    - ### Antes de prosseguir com a última linha, siga os comandos abaixo:
    ```
    git status 
    git add .
    git commit -m "seu commit" 
    ```
    - ### Após isso, pode finalmente dar o comando final de push. Mais sobre os comandos pode ser visto no arquivo de [comandos básicos](./comandosGit.md). 

***

- ## Clonou um repositório já pronto e deseja subir suas alterações
    - ### Para clonar um repositório, siga o comando abaixo no gitbash/terminal 
    ```
    git clone <repositorio(link)>
    ``` 
    - ### Coloque esse comando no git bash que você abrir onde deseja clonar o repositório.
    - ### Após isso, entre na pasta e tenha certeza que a pasta .git aparece para você. Caso não, vá em exibir na superior ao lado de compartilhar, na pasta, e selecione a caixinha de itens ocultos. Um tutorial pode ser observado [aqui.](https://support.microsoft.com/pt-br/windows/exibir-pastas-e-arquivos-ocultos-no-windows-97fbc472-c603-9d90-91d0-1166d1d9f4b5)
    - ### Essa pasta .git é responsável por armazenar os logs dos commits, então é extremamente importante não apagar ou fazer git init por cima da pasta. 
    - ### Faça todas alterações desejadas. Ao fim, abra o git bash/terminal na pasta onde se encontra o .git. Caso deseja colocar o .gitignore, coloque nessa pasta. Assim, faça esses comandos para validar suas alterações: 
    ```
    git status 
    git add .
    git commit -m "seu commit" 
    ```
    - ### segue a vida feliz.

*** 

- ## Deseja criar um repositório do início
    - ### Para isso, clique em criar repositório no github e siga a primeira instrução do site. 
    ```
    echo "# git-documentation" >> README.md
    git init
    git add README.md
    git commit -m "first commit"
    git branch -M main
    git remote add origin https://github.com/sabrinahelena/git-documentation.git
    git push -u origin main
    ``` 
    - ### Essas instruções irão criar um readme.md para você, dar o git init para inicializar o git, adicionar, comitar, trocar para a branch main, adicionar o remoto e depois dar push na origin main. 