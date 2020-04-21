Git 

Commit
push
pull

// configura nome e email global 
git config --global user.name nome
git config --global user.email email

git config --global --list // mostra configurações globais

 
git init //iniciar repositorio
git status // status daquele momento
rm -rf .git/ // deleta repositorio e perde commits

// primeiros commits
git add nome do arquivo // adiciona o arquivo para o stage ( git 'cuida')
git add. pega todos os arquivos de uma vez e coloca na stage
git  commit -m "mensagem" //comita
git  commit -am "mensagem //arquivo modificado pra comitado

git log // mostra todos os comits
git log --oneline // mostra commits simplificados
git log -(numeros dos ultimos commits a serem mostrados) //mostra os ultimos n commits
git log -1 --stat //mostra quantas linhas adicionadas e excluidas
git log --author=nome do autor // mostra commit do autor

git show (hash) //mostra o que aconteceu com o commit

.gitignore // cria diretorio do git para ignorar arquivos no commit

git diff (arquivo)//mostra a diferença entre um arquivo e o seu estado anterior
git diff --staged 
git diff hashpai..hasfilho // mostra as alterações entre os commits


git checkout --arquivo // discarta alterações que não foram para o stage
git reset --arquivo // tira o arquivo da stage
git reset --soft hash_pai // pega o arquivo comitado e volta pra stage
git reset --mixed hash_pai // pega o arquivo comitado e volta pra modified
git reset --hard hash_pai // apaga o comit e as alterações
git revert hashdocommit "mensagem" ou --no-edit // faz revert do commite
git rm nome do arquivo// deleta tudo arquivo e modificações dos filhos
git mv nomeantigo nomenovo // muda nome arquivo


git remote add origin urldogit//ligar o git no repositório do github
git remote // verifica onde está conectado o repositorio
git remote -v //mostra o url do repositório
git push origin master // sobe os arquivos pro git
git pull origin master // pega o repositorio atualizado do git

git clone url nome(nome do repositorio opcional) // clona um repositorio do git