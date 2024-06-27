# Git e GitHub

## Ferramenta para visualizar o funcionamento do Git

[Git Visualization](https://git-school.github.io/visualizing-git/)

### git log
Exibe o histórico de commits do repositório, mostrando informações detalhadas como o hash do commit, o autor, a data e a mensagem do commit.

### git log --oneline
Mostra o histórico de commits de forma resumida, exibindo cada commit em uma única linha com o hash abreviado e a mensagem do commit.

### git log -p
Exibe o histórico de commits juntamente com as diferenças introduzidas em cada commit, mostrando as alterações de código linha por linha.

### git log --graph
Mostra o histórico de commits com uma representação gráfica das ramificações e fusões do repositório, facilitando a visualização da estrutura do repositório.

### git log --format="%H %an"
Personaliza a saída do histórico de commits, exibindo apenas o hash completo do commit e o nome do autor.

### git show `hash_do_commit`
Exibe as informações detalhadas de um commit específico, incluindo as alterações de código, a mensagem do commit e os metadados associados.

### git `comando` --help
Mostra a página de ajuda e documentação detalhada do comando Git especificado.

### git status
Exibe o estado atual do repositório, mostrando quais arquivos foram modificados, adicionados ou removidos, e quais estão prontos para o commit.

### git add `nome_do_arquivo`
Adiciona o arquivo especificado à área de stage, preparando-o para o próximo commit.

### git commit -m `descricao`
Cria um commit com as alterações atualmente na área de stage e associa uma mensagem descritiva ao commit.

### git diff
Mostra as diferenças entre as alterações não comitadas e a última versão comitada do repositório.

### git checkout `nome_da_branch`
Muda para a branch especificada, atualizando o diretório de trabalho para refletir o estado dessa branch.

### git branch -d `nome_da_branch`
Deleta a branch especificada do repositório local.

### git switch -c `nome_da_branch`
Cria uma nova branch com o nome especificado e muda para essa nova branch.

### git merge `nome_da_branch`
Combina as alterações da branch especificada na branch atual, mesclando os históricos de commits.

### git rebase `nome_da_branch`
Aplica os commits da branch atual sobre a branch especificada, criando uma história de commits linear.

### git stash push -m `descricao_do_stash`
Salva as alterações atuais em um stash com uma descrição, permitindo que você retorne a um estado de trabalho limpo.

### git stash pop
Aplica as alterações mais recentes do stash ao diretório de trabalho e remove essa entrada do stash.

### git stash list
Lista todos os stashes salvos, mostrando suas descrições e índices.

### git stash apply `indice`
Aplica as alterações de um stash específico ao diretório de trabalho sem remover a entrada do stash.

### git stash clear
Remove todos os stashes salvos do repositório.

### git restore `nome_do_arquivo`
Restaura o conteúdo do arquivo especificado para o estado da última versão comitada.

### git restore --staged `nome_do_arquivo`
Remove o arquivo especificado da área de stage, desfazendo `git add` para esse arquivo.

### git restore --source=`id_commit` `nome_do_arquivo`
Restaura o arquivo especificado para o estado de um commit específico.

### git tag `nome_da_tag` `id_commit`
Cria uma tag leve com o nome especificado associada ao commit especificado.

### git push origin `nome_da_tag`
Envia a tag especificada para o repositório remoto.

### git tag -a `nome_da_tag` -m `mensagem da tag`
Cria uma tag anotada com o nome especificado e uma mensagem associada ao commit atual.

### git tag -d `nome_da_tag`
Deleta a tag especificada do repositório local.

### git cherry-pick `id_commit`
Aplica as mudanças de um commit específico na branch atual.

### git blame `nome_do_arquivo`
Mostra informações sobre cada linha do arquivo especificado, incluindo o commit, o autor e a data de modificação.

### pwd
Mostra o diretório atual.

### cd /diretório
Entra em um determinado diretório.

### ls
Mostra os arquivos do diretório.

### mkdir nome_diretório
Cria um diretório.

### touch nome_arquivo
Cria um arquivo.

### git init
Cria um repositório local no diretório escolhido.

### ls -a
Exibe o diretório oculto .git.

### git add nome_do_aquivo.tipo
Adiciona um arquivo ao repositório.

### git add *
Adiciona todos os arquivos ao repositório.

### git add .
Adiciona todos os arquivos ao repositório.

### git commit -m "Comentários"
Serve para identificar o contêiner e armazenar os arquivos no repositório.

### git log --oneline --graph
Mostra os grafos de commits.

### git commit -am "Comentários"
Adiciona o arquivo ao contêiner e cria o commit.

### git branch
Informa o ramo em que o projeto se encontra.

### git checkout "código do log --oneline"
Comando de backup, serve para acessar versões anteriores do projeto e alternar entre os ramos.

### git reset --hard 'hash_versão_anterior'
Remove os commits retornando-o para versão apontada.

### git log --oneline --graph --all
Mostra todo o grafo com suas ramificações e merges realizados.

### git remote add origin https://github.com/usuário_do_github/repositório_do_github
Adiciona o repositório de projetos do Git local para o remoto no GitHub.

### git remote
Informa o repositório remoto adicionado.

### git remote -v
Traz informações sobre o repositório remoto adicionado.

### git push -u origin master
Faz o upload dos arquivos do repositório local para o repositório remoto.

### git push
Faz o upload dos arquivos do repositório local para o repositório remoto.

### git clone "link_do_repositorio_gerado_no_site_do_GitHub"
Cria um clone do repositório do GitHub no diretório desejado.

### cd ..
Retorna a um diretório um nível acima.

### git pull
Faz o download de todas as alterações realizadas diretamente no repositório remoto para o repositório local.

### git fetch
Utilizado para fazer o download das alterações que estão no repositório remoto para poder ser realizada uma análise do que foi modificado e resolver problemas de conflito. Equivale ao `git pull`, porém ele não realiza o merge. Quando for dado o comando `git fetch`, é necessário direcionar-se ao diretório remoto para realizar as análises, então após dado o `git fetch`, utiliza-se em conjunto o `git remote`, `git checkout origin` (verificar as alterações). Depois de verificar as mudanças, `git checkout master`, `git pull`. Depois disso, ele vai informar quais os problemas de conflitos a serem resolvidos.

### git rm --cached nome_do_arquivo
Remove o arquivo do contêiner.
