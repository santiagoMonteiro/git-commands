# GIT

git init
git add <nome-do-arquivo-a-ser-adicionado-a-stage-area>
git commit -m "<mensagem-do-commit>"
git log // para visualizar os pontos na história
git status verificar stage area e arquivos não rastreados
 
git show <hash-do-commit> // mostrar o commit
git show // Mostrar o último commit

git branch <nome-da-branch> // para criar branch nova
git branch // mostrar as branches existentes
git branch -D <nome-da-branch> // deletar branch
git branch -a // mostrar branches remotas
git checkout <nome-da-branch> // para mudar para uma branch especifica
git checkout -b <nome-da-branch> // criar branch e mudar para ela
git checkout <hash-do-commit> -- {nome do arquivo} // recuperar arquivo
git merge <nome-da-branch-a-se-juntar> // para juntar branches


git remote add origin <url.git> // adicionar repositório remoto
git remote -v // listar repositórios remotos

git push origin main
git pull

git clone {url do repositorio} # clonar repositorio
git clone git@hostname:company/project.git # clonar repositório com host específico
git clone -b <branchname> <remote-repo-url> # clonar branch específica

git reset --soft <hash>
// --soft: // voltar ao commit com as mudanças atuais no stage area
// --mixed: // voltar ao commit com as mudanças atuais fora do stage area
// --hard: // voltar ao commit sem nenhuma modificação atual,
          // e os commits que vieram depois somem

git diff // diferenças entre estado atual e último commit
git diff --name-only // nome dos arquivos que foram modificados
git diff <nome-do-arquivo> // diferença referente a um arquivo específico
git checkout HEAD -- <nome-do-arquivo> // retirar as alterações atuais
 
git pull origin master --allow-unrelated-histories // fazer o pull quando o merge é impossibilitado

git fetch // atualizar com as branches remotas
git fetch -p // atualização juntamente com as branches deletadas

