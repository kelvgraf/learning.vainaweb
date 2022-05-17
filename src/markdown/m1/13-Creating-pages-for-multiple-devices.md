---
slug: "/module-1/creating-pages-for-multiple-devices"
date: "2022-17-05"
title: "13 - Criando páginas para múltiplos dispositivos"
id: 13
category: "module-1"
---

# Criando páginas para múltiplos dispositivos

Muita coisa aconteceu desde o surgimento da internet, e nossa experiência com a tecnologia também se modificou muito com o passar dos anos. A realidade que conhecemos hoje, é que estamos realmente conectados o tempo inteiro, e através de vários dispositivos diferentes.

Não somente no computador, hoje sabemos que é possível nos conectar usando uma infinidade de aparelhos diferentes, televisão, videogame, celular, etc. E estamos conectados também nos mais diferentes lugares, seja na padaria, na escola, ou em casa. A web está em todos os lugares!

É nosso dever e desafio enquanto desenvolvedores web, criar páginas que possibilitem que essas experiências aconteçam da melhor forma possível. Há muitas coisas que podemos fazer para garantir que isso aconteça, uma delas, é criar páginas que sejam exibidas de forma correta nos mais diferentes dispositivos, assim nasceu o conceito de Design responsivo.

Dizemos que uma página é responsiva, quando os elementos dela se adaptam automaticamente à tela do dispositivo no qual ela está sendo visualizada. Na prática, há algumas técnicas que usamos para que esse comportamento aconteça.

Antes de tudo, precisamos dizer ao navegador que a escala inicial da nossa página é equivalente ao tamanho do dispositivo. Adicionamos a seguinte linha ao *head*:

```html
<head>
    ...
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    ...
</head>
    
```

Nós já aprendemos Flexbox, então todo o resto acaba por ficar mais simples a partir daqui. Isso porque o Flexbox é muito legal para tornar nosso layout flexível, isso porque flexibilidade e fluidez fazem parte do que queremos atingir com o design responsivo. Ao invés de ficar usando pixels, nós também podemos usar unidades de medida flexíveis.

Também muito importantes para tornar nossas páginas responsivas são as media queries. Usamos elas basicamente para criar modificações na página para que ela se adapte de acordo com uma medida. Nós podemos dizer por exemplo que se uma página tem até 640px de largura o background dela deve mudar sua cor.

```css
@media (max-width: 768px) {
    body {
        background: deepskyblue;
    }
}
```

Mudar a cor de uma página de acordo com seu tamanho pode não ser muito interessante, mas podemos modificar outras coisas que são, como por exemplo modificar o tamanho de um container, o lugar de um botão, deixar uma letra maior ou menor... são muitas possibilidades que podem e devem ser aproveitadas.

Para escolher que parâmetros usar na media query podemos usar várias propriedades, como o width, height, orientation, aspect-ratio, color, monochrome, resolution, etc. Há duas propriedades principais que as pessoas preferem usar, são a max-width e a min-width.

No exemplo que usamos anteriormente usamos o conceito de desktop-first, onde assumimos que todo o CSS que já escrevemos foi feito para o desktop, e então adicionamos algumas media querys para tamanhos menores de tela. Quando usamos max-width 640px estamos dizendo que essas modificações do bloco de dentro da media query serão usadas em dispositivos com até 640px de largura.

Se optarmos por seguir o conceito de mobile-first, assumimos que o CSS atual foi pensado em medidas menores, perfeitas para o mobile, temos agora que adicionar algumas media querys para tamanhos maiores de tela. Exemplo:

```css
@media (min-width: 640px) {
    body {
        background: deepskyblue;
    }
}
```

Nesse exemplo, a tela só ficará azul em dispositivos com telas a partir de 640px de largura. Basicamente, enquanto no desktop-first pensamos em modificações para telas menores, no mobile-first pensamos em maiores.

De acordo com cada centário, podemos considerar muitas coisas, e pensando nessas coisas usar as melhores técnicas para criar a experiência de navegação que queremos.


![bye bye](https://media.giphy.com/media/42D3CxaINsAFemFuId/giphy.gif)

