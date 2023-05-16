# learn_git_and_github
Aprendendo como usar todos os recursos do git + github

## o que é git?
git é um sistema de versionamento de arquivos.

## primeiros passos

- indique ao git quem está fazendo as modificações:
```bash
$ git config --global user.name "<coloque seu username do github>"
$ git config --global user.email "<coloque o email cadastrado no github>"
```

precisamos agora criar uma chave ssh para realizarmos clones dos nossos repositórios. para isso, basta seguir este rápido [tutorial](https://docs.github.com/pt/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent) do próprio github.

com a cheva ssh configurada no seu git, podemos clonar qualquer repositório. para isso basta copiar o link que corresponde ao ssh e executar o seguinte comando:

```bash
$ git clone <url>
```

## comandos básicos do git
### git add

o `git add` é um comando para adicionar arquivos para uma base do git. pensando assim poderá ajudá-lo: "estou colocando arquivos em uma caixa".
para usar este comando faça:

```bash
$ git add <arquivo>
```

uma prática comum é ao invés de adicionar arquivo por arquivo é usar a tag `-A ou -all` desta forma:
```bash
$ git add -A
```
isso irá adicionar todos os arquivos para a "caixa".

### git status

o comando `git status` é um comando que seguindo nossa analógia, ele indicará com a cor **verde** osarquivos que estão dentro da caixa e **vermelho** para arquivos que não foram adicionados na caixa.

### git commit

o comando `git commit` é um comando que salva as modificações que foram adicionadas na "caixa".
para usá-lo:
```bash
$ git commit -m "<mensagem>"
```
na estrutura do comando, a flag `-m` indica uma mensagem que e colocada logo em seguida entre aspas "". é recomendável que essa mensagem indique o que foi realizado nas modificações salvas.

### git push

o comando `git push` realiza a entrega da "caixa" para o github. para usá-lo:
```bash
$ git push <remote> <branch>
```
no caso, o remote e o repositório remoto que foi configurado, geralmente o origin. a branch é o nome da ramificação. 
para casos simplificados, em que só se tem uma branch, geralmente a main/master, usamos apenas:
```bash
$ git push
```

### git pull
o git pull é o comando git responsável por puxar todos as mudanças feitas no repositório remoto.

## clonado uma branch
para clonar uma branch especifica use o seguinte comando:
```bash
$ git clone -b <nome da branch do remoto> <url>
```

## fazer o push para a branch clonada:
para realizar o push na branch especifica use o comando abaixo:
```bash
$ git push <repositório remoto> <branch local>:<branch remota>
```

para verificar como o repositório remoto esta nomeado use:
```bash
$ git remote
```
para saber a branch local use:
```bash
$ git branch
```
