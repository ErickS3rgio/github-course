GitHub
Arquivo da aula de Git e GitHub para iniciantes
Este é um arquivo para observar como o Git funciona.

Adicionando um Link ...

git log //Comando usado para descrever as modificações comitadas assim como seus autores.
Existem também opções de git log como:
git log --decorate //Que mostra as tags que foram geradas, os merges*/
git log --author="(nome a ser feita a busca)" //Que busca por comites que foram realizados por autores do parâmetro.

git shortlog //Mostra qual foram os autores, quantos comites fizeram e os arquivos criados/modificados e as suas respectivas mensagens
git shortlog -sn //Mostra apenas os nomes e a quantidade de comites feitos por cada colaborador

git log --graph //Mostra em forma grafica as modificações feitas pelos colaboladores no arquivo.

git show '(hash(tag) de caracteres usados como índice para controle do versionamento)'//Mostra as informações do que foi adicionado

git status //mostra no prompt se há algum arquivo para ser gravado e mostra em qual estado este arquivo está.

git diff //Mostra a última modificação feita no arquivo
git diff --name-only //Mostra apenas o nome do último arquivo modificado

git checkout (nome do arquivo) // Retorna o arquivo para o estado antes da última edição (Antes de adicionar o arquivo para a área de 'Unstage')

git reset HEAD (nome do arquivo) //Retorna o arquivo para um estado antes de 'Unstage'
git reset --soft (hash(tag) do commite anterior ao que deseja voltar) //Retorna o arquivo para o estado 'Unstage'
git reset --mixed (hash(tag) do commite anterior ao que deseja voltar) //Retorna para o estado onde é possivel ver qual foi a última alteração, (tipo git diff)
git reset --hard (hash(tag) do commite anterior ao que deseja voltar) //Mata o último commite feito e o HEAD passa a ser o estado do penúltimo commite com sucesso.

//Aprendendo a usar um pull request. 
git push origin master // push aloca em 'origin' no branch 'master'

//Aprendendo a clonar um repositório 
git clone 'nome do repositório' (nome da pasta a ser copiado o arquivo)

Aprendendo a diferença entre um 'git clone' e um 'fork'
git clone // clona um repositório para ser usado na sua máquina, porém não é possivel subir para o github
Usar o fork possibilia que seja possível copiar um repositório adicionar mudanças e requisitar que o dono original do repositório aceite ou não as mudanças
