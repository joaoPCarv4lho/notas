# **Inicializando Git Local**

Primeiro confira se o Git está instalado:
``` bash
git --version
```
Se o Git estiver instalado configure seu usuário e seu e-mail:
```bash
git config --global user.name "seu nome"
git config --global user.email "seuemail@gmail.com"
```
Agora que você tem seu usuário e email configurados, para inicializar o local basta executar os seguintes comandos:
```bash
cd Documents
mkdir NomeDaSuaPasta
git init
```
# **COMANDOS DO GIT**

```
git status 
```
- Exibe os caminhos que têm diferenças entre o arquivo índice e o commit atual no Head, os caminhos que têm diferenças entre a árvore de trabalho e o arquivo do índice, os caminhos na árvore de trabalho que não são rastreados pelo Git;


&nbsp;
```
git-add <filename ou . >
``` 
- Este comando atualiza o índice usando o conteúdo atual encontrado na árvore de trabalho, para preparar o conteúdo preparado para o próximo commit. Ele normalmente adiciona o conteúdo atual dos caminhos existentes como um todo, mas com algumas opções também pode ser usado para adicionar conteúdo com apenas parte das alterações feitas nos arquivos da árvore de trabalho aplicados ou remover caminhos que não existem na árvore de trabalho não mais;


&nbsp;
```
git-restore --staged
```
- Restaura os caminhos definidos na árvore de trabalho com algum conteúdo de uma fonte de restauração. Se um caminho for monitorado, porém não existir na fonte de restauração, ele será removido para coincidir com a fonte.O comando também pode ser usado para restaurar o conteúdo no índice com a opção --staged;

&nbsp;
```
git branch <branchname>
```
- Lista, cria ou exclui ramificações;


&nbsp;
```
git branch -D <branchname>
```
- Um atalho para --delete --force.


&nbsp;
```
git-checkout <branchname>
```
-  Alterna ramificações ou restaurar arquivos da árvore de trabalho;


&nbsp;
```
git-checkout -b <branchname>
```
- Usando a opção -b faz com que um novo ramo seja criado;


&nbsp;
```
git commit -m "<description>"
```
- Grava as alterações para o repositório. Usa a *descripition* como a mensagem de commit. Caso múltiplas opções -m sejam usadas, o seu conteúdo será disposto em parágrafos separados.


&nbsp;
```
git push
```
- Atualiza os refs remotos através da associação dos objetos.


&nbsp;
```
git-pull
```
- Capture de e o integre com um outro repositório ou em um outro ramo local.


&nbsp;
```
git fetch
```
- Faz o download dos objetos e dos refs vindo de outro repositório.

  # ENVIANDO UM REPOSITÓRIO LOCAL PARA O GITHUB


&nbsp;
- Abra o arquivo que será empurrado para o GitHub no seu ambiente de desenvolvimento, (no meu caso utilizei o VsCode). Depois de abrir o se arquivo, abra o terminal(Ctrl + Shift +') ou você pode abrir direto pela barra de opções do VsCode clicando em Terminal > Novo Terminal. Após ter feito esse processo, digite o seguinte comando no terminal:
```
git status
```
Esse comando irá mostrar se o documento já foi commitado ou não. A seguir, execute o próximo comando:
```
git add .
```
Você irá atualizar e preparar o conteúdo para o próximo commit.


&nbsp;
- O próximo passo será executar o comando ```git commit -m "<descripition>"``` para gravar as atualizações no repositório,( lembre de colocar uma descrição decente pois o repositório será público).


&nbsp;
- Após esse passo a passo, você será redirecionado para o seu browser, basta apenas habilitar as autorizações e logo em seguida você será direcionado para sua conta do GitHub. E pronto, você conseguiu fazer o seu primeiro commit de muitos!
