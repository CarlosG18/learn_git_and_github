# learn_git_and_github
Aprendendo como usar todos os recursos do git + github

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

## usando uma nova branch
- modificando o Readme.md
