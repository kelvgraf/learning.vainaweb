---
slug: "/module-1/command-line-intro"
date: "2022-17-05"
title: "11 - Conhecendo a linha de comando"
id: 11
category: "module-1"
---

# Conhecendo a linha de comando

Vamos conhecer finalmente a famosa telinha preta que vemos os hackers usando nos filmes e séries. Algo que o cinema não mostra, é que elas são bem simples, e podem ser usadas para diversas coisas, como criar um novo arquivo, e até mesmo colocar um site ou aplicação online.

```
$ sudo apt install amorrr
```

Essa famosa tela preta, que é chamada de linha de comando, cmd, prompt, console, terminal... ufa! ou interface de linha de comando, é um aplicativo baseado em texto para visualização, manipulação e manuseio de arquivos em seu computador.

##Primeiros comandos
Vamos aprender alguns comandos, eles mudam um pouco de sistema operacional para sistema operacional. Durante essa aula vamos focar nos comandos do Linux. Isso porque nos computadores dos polos onde o VnW acontece escolhemos usar esse sistema.

Mas se você usa Windows em casa pode pesquisar os comandos equivalentes, ou se preferir, você pode instalar o [Git Bash](https://git-scm.com/) mas nem todos os comandos podem funcionar.


Para começar, abra o terminal digite o seguinte comando:

```
$ whoami
```

Seria legal saber em que pasta estamos agora. É recomendável que você sempre saiba essa informação! Se você não souber, é só usar o comando. Digite o seguinte comando e aperte o enter:

```
$ pwd
```

Se preferir, você pode também se localizar vendo quais arquivos estão dentro da pasta. Você pode descobrir isso usando o comando para listar arquivos:

```
$ ls
```

## Navegando entre pastas

Uma coisa bem legal que você pode fazer agora é aprender a navegar entre pastas! Eu não tenho certeza de quais pastas você tem aí em seu computador, então vamos criar uma nova chamada teste. Digite o seguinte comando:

```
$ mkdir teste
```

Para ter certeza de que a pasta foi criada você pode usar o ls novamente.

```
$ ls
```

Se a pasta foi criada, agora você pode entrar dentro dela usando o seguinte comando:

```
$ cd teste
```

Legal! Você conseguiu entrar dentro dela. E se quisermos também criar um novo arquivo em nossa pasta nova? Vamos criar um chamado texto.txt usando o comando touch:

```
$ touch texto.txt
```

Que tal agora voltar? Você pode fazer isso usando o comando:

```
$ cd ..
```

## Mais alguns comandos

Há muitos comandos úteis, que podem fazer muitas coisas, como desligar o computador, criar arquivos, remover arquivos, e mais um monte de outras coisas. Há alguns bem básicos que podem nos ajudar muito em nossas tarefas enquanto desenvolvedor. Vamos conhecer alguns:

```
Comando - Windows   |   Comando - Mac OS / Linux     |   Descrição
--------------------|--------------------------------|----------------------------------
exit                |   exit                         |   Fecha a janela
cd                  |   cd                           |   Muda a pasta
ls                  |   pwd                          |   Mostra o diretório atual
dir                 |   ls                           |   Lista as pastas e/ou arquivos
copy                |	cp                           |   Copia um arquivo
move                |   mv                           |   Move um arquivo
mkdir               |   mkdir                        |   Cria uma pasta
rmdir (ou del)	    |   rm                           |   Exclui arquivo
rmdir /S            |   rm -r                        |   Exclui diretório
```


![bye bye](https://media.giphy.com/media/42D3CxaINsAFemFuId/giphy.gif)

