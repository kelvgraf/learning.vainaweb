---
slug: "/module-1/html-forms"
date: "2021-02-05"
title: "03 - HTML na prática: Forms"
id: 3
category: "module-1"
---

# 03 - HTML na prática: Forms

## O que é um form?

A tag **form** \(formulário\) é utilizada para agrupar elementos interativos, onde o usuário vai inserir informações que serão enviadas para um servidor. As tags mais comuns utilizadas em formulários são:

1. \<label\>
2.  \<input\>
3.  \<button\>

Exemplo de um formulário html:

```html
<form>
  <label for="name">Name:</label>
  <input id="name" type="text" name="name" placeholder="escreva seu nome">
  <input type="submit" value="Save">
</form>
```

Vamos quebrar esse código em partes:

1. Marcando nosso formulário: 

```html

<form>

</form>
```

Primeiro criamos uma tag **form** que será responsável por agrupar todos os campos e buttons que iremos usar.

2. Criando uma legenda visível:

```html
<label for="name">Name:</label>
```

Agora criamos uma tag **label** que é usada como legenda para a tag **input** que vamos usar no próximo passo.

3. Criando o primeiro input:

```html
<input id="name" type="text" name="name" placeholder="escreva seu nome">
```

Usamos a tag **input** para criar um campo onde o usuário pode digitar as informações pedidas no formulário. 

Esse campo pode receber diferentes tipos de dados: text, email, password, number, tel, por exemplo. 

No nosso caso o **input** tem o tipo **"text"**, notem também que usamos um atributo chamado **placeholder** que é utilizado para exibir um texto dentro do campo enquanto ele está vazio.

4. Criando um botão:

```html
<input type="submit" value="Save">
```

Por último temos um **input** com um type especial chamado **submit**, esse **input** é utilizado para submeter \(enviar\) o formulário para um servidor quando ele é clicado. Na prática ele é um **button** que envia todos os dados escritos nos campos para algum servidor.

Agrupando todas essas tags nós temos nosso primeiro formulário pronto :)

```html
<form>
  <label for="name">Name:</label>
  <input id="name" type="text" name="name" placeholder="escreva seu nome">
  <input type="submit" value="Save">
</form>
```

### Há ainda muitos atributos úteis que não vimos ainda, por agora, veremos mais alguns dos mais usados.

1. \<textarea\>
2. \<input type="radio"\>
3. \<input type="checkbox"\>
4. \<select\>
5. \<fieldsets\>
6. \<legend\>

<!--  -->

5. Criando o primeiro textarea:

Diferente do input, esse elemento pode aceitar textos maiores, ideal para quando queremos receber um texto com mais de uma linha.Ele aceita apenas um tipo de valor, o atributo name.

```html
<form>
  ...
    <textarea name="comentario">
      Deixe aqaui seu comentaario...
    </textarea>
  ...
</form>
```

6. Criando  Botão Radio:

Parar cria-lo, usamos o input, e adicionamos o type radio. É necessário que todos os botões do conjunto tenham o mesmo name.Com botões de rádio, um usuário faz uma seleção de múltipla escolha. Assim, temos que definir o valor de entrada. Usando o atributo de value, podemos definir um valor específico para cada elemento input.

```html
<form>
  ...
   <input type="radio" name="dia" value="Segunda"> Segunda
   <input type="radio" name="dia" value="Sabado"> Sábado
   <input type="radio" name="dia" value="Domingo"> Domingo
  ...
</form>
```

É possível também pré-selecionar um botão de opção para o usuário, podemos usar o atributo checked.

```html
<form>
  ...
   <input type="radio" name="dia" value="Segunda"> Segunda
   <input type="radio" name="dia" value="Sabado" checked> Sábado
   <input type="radio" name="dia" value="Domingo"> Domingo
  ...
</form>
```

7. Criando  Checkbox:

Usamos os mesmos atributos e padrões do radio buttons, mas para usá-lo mudamos o valor do type para checkbox.Com o checkbox, os usuários podem selecionar vários valores.

```html
<form>
  ...
   <input type="checkbox" name="dia" value="Segunda" checked> Segunda
   <input type="checkbox" name="dia" value="Sabado"> Sábado
   <input type="checkbox" name="dia" value="Domingo"> Domingo
  ...
</form>
```

8. Criando Select e Option:

Para cria-la usaremos os elementos select e option. O elemento select envolve todas as opções.Cada opção é marcada usando o elemento option. 
Cada elemento da lista fica em um option. Ao invés de checked, para pré-selecionar uma opção usamos o selected como atributo na opção que queremos fazer isso.

```html
<form>
  ...
   <select name="dia">
     <option value="Segunda">Segunda</option>
     <option value="Sabado">Sábado</option>
     <option value="Domingo" selected>Domingo</option>
   </select>
  ...
</form>
```

9. Criando Fieldsets:

Usamos Fieldsets para agrupar os controles de formulário e os rótulos em seções organizadas. Assim como uma section, fieldset é um elemento de nível de bloco que envolve elementos relacionados dentro de um form, para melhor organização.

```html
<form>
  ...
  <fieldset>
    <label>
      Usuário
      <input type="text" name="Usuario" placeholder="Usuário">
    </label>
     <label>
      Senha
      <input type="password" name="Password" placeholder="Digite sua senha">
    </label>
   </fieldset>
  ...
</form>
```

10. Criando Legend:

Legend funciona como um título para o fieldset, ele pode envolver uma descrição dos controles do fieldset.

```html
<form>
  ...
  <fieldset>
    <legend>Login:</legend>
    <label>
      Usuário
      <input type="text" name="Usuario" placeholder="Usuário">
    </label>
     <label>
      Senha
      <input type="password" name="Password" placeholder="Digite sua senha">
    </label>
   </fieldset>
  ...
</form>
```

11. Outros

Para desabilitar um campo por exemplo, usamos o atributo disabled.Para mostrar uma descrição do controle dentro do próprio campo input usamos o placeholder.Para tornar o preenchimento do campo como obrigatório usamos o required.


![thanks](https://media.giphy.com/media/psmj7c3DbrJKkbRYFj/giphy.gif)

