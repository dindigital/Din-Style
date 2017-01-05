# Din Style

Framework CSS da Din Digital. A documentação você pode ver [aqui](https://github.com/dindigital/style-patterns/wiki) e os exemplos você pode ver [aqui](http://nncl.github.io/Din-Style/).

## Sass

O framework utiliza o Sass como pré-processador CSS, na extensão `.scss`.

### Instalação

Para utilização do arquivo `.css` e também para edição/utilização do arquivo `.scss`.

#### Via bower
`bower install din-style --save`

#### Sass
Para os usuários de MAC é bem mais tranquilo que para os usuários de PC, porque para o Sass “rodar“ precisamos que o Ruby também esteja instalado e isso já é nativo no MAC. De qualquer forma, não é nenhuma experiência traumática. No próprio site do Sass [você encontra os dois métodos de instalação](http://sass-lang.com/install).

Para MAC, abra o terminal e entre no repositório do framework. Depois é só rodar o comando:

`sass --watch style.scss:style.css`

Este comando cria um novo arquivo `style.css` no mesmo diretório traduzindo as linhas digitadas em `.scss` para `.css`.

## Atualização do Repositório e Bower

Vamos supor que vamos fazer uma alteração no DS e que agora vai sair a versão 1.1.x. A primeira coisa a se fazer é editar o arquivo bower.json. Devemos atualizar o "version" do arquivo para "1.1.6". Exemplo:

```
{
  "name" : "din-style-framework",
  "version" : "1.1.x"
  ...
}
```

Em seguida, devemos comitar a atualização:

```
git add .
git commit -m "Nova versão"
```

E após, taggear o commit da nova release:

```
git tag -a v1.1.x -m "Release versão 1.1.x"
```

E por fim, subir a nova versão para as branchies master e tag 1.1.6:

```
git push origin master --tags
```
