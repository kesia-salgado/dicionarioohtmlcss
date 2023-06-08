# Dicionário de Termos HTML e CSS Básicos
Ou um pouco de facilidade para quem está começando agora. Afinal de contas, nós merecemos.

Conheça mais o meu trabalho e dê um like https://www.linkedin.com/in/kesiasalgado.

Aqui está um pequeno dicionário com os termos básicos relacionados ao HTML e CSS, destinado a devs iniciantes.

## HTML (HyperText Markup Language)

**1. Tag**: Um elemento de marcação usado para estruturar e apresentar o conteúdo em um documento HTML.
Caso você deseje adicionar um paragrafo na sua plataforma é só colocar a **TAG** de parágrafo como vemos abaixo:
```<p>Este é um exemplo de parágrafo HTML.</p>```

**2. Elemento**: Uma combinação de uma tag de abertura, conteúdo e uma tag de fechamento, que juntos formam uma unidade no documento HTML.
Neste exemplo, a tag `<a>` é usada para criar um link, onde o atributo `href` define o URL de destino e o texto "Clique aqui" é exibido como o texto âncora do link.
`<a href="https://www.example.com">Clique aqui</a>` 

**3. Atributo**: Informações adicionais fornecidas nas tags HTML para modificar o comportamento ou a aparência dos elementos.
Exemplo de atributo HTML:

No exemplo abaixo, o atributo `src` é usado na tag `<img>` para especificar o caminho da imagem a ser exibida:

`<img src="caminho-da-imagem.jpg" alt="Descrição da imagem">`

Neste caso, o atributo `src` define o caminho da imagem e o atributo `alt` fornece uma descrição alternativa para a imagem.

**4. Elemento de Bloco**: Um elemento que ocupa toda a largura disponível e inicia uma nova linha no documento HTML, como `<div>`, `<p>`, `<h1>`-`<h6>`, etc.
Para o exemplo de elemento de bloco iremos utilizar a `<div>` conforme abaixo:
```
<div>
  <h2>Título do Parágrafo</h2>
  <p>Este é um parágrafo de exemplo.</p>
</div>
```
Neste exemplo, a tag <div> é usada para criar um contêiner/elemento de bloco.
Aqui neste link você pode conhecer mais sobre os elementos de conteiner do HTML: https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element

**5. Elemento Inline**: Um elemento que ocupa apenas o espaço necessário e não inicia uma nova linha, como `<img>`, `<a>`, `<strong>`, etc.
Exemplo de elemento HTML inline 
 `<img>` da seguinte forma: <img src="caminho-da-imagem.jpg" alt="Descrição da imagem">

Neste exemplo, a tag <img> é usada para exibir uma imagem inline. O atributo src especifica o caminho da imagem e o atributo alt fornece uma descrição alternativa para a imagem.

**6. ID**: Um atributo exclusivo atribuído a um elemento HTML para identificá-lo de forma exclusiva em uma página.
Vemos o exemplo abaixo:
```<a href="#titulo-principal">Ir para o Título Principal</a>```

Isso significa O uso do id permite que você faça referência a esse elemento em outros lugares do documento HTML ou até mesmo em folhas de estilo CSS. Por exemplo, você pode criar um link que aponte diretamente para o título principal da página usando a **TAG** (<a>) e o id.

**7. Classe**: Um atributo atribuído a um ou mais elementos HTML para agrupá-los e estilizá-los de forma conjunta com CSS.
Criamos aqui um exemplo para atribuir uma classe dentro da **TAG** <p> (parágrafo):

```<p class="destaque">Este é um parágrafo de exemplo com classe.</p>```

A classe pode ser utilizada para aplicar estilos CSS específicos a esses elementos ou selecioná-los com JavaScript para realizar ações personalizadas.

Assista aqui a estilização de uma classe no CSS: https://www.youtube.com/watch?v=YgEp4Qt1NqE.

**Agora vamos entender um pouco sobre a estilização do html.**

## CSS (Cascading Style Sheets)

**1. Seletor**: Ele permite selecionar elementos HTML com base em seus nomes de tag. 
A estrutura do seletor é feito da forma a seguir: 
```
p {
  color: blue;
}
```

Dentro do seletor você pode adicionar propriedades e valores na tag selecionada.

**2. Propriedade**: Uma característica de estilo específica que pode ser aplicada a um elemento HTML, como `color`, `font-size`, `margin`, etc.
Que pode ser utilizada de forma individual para cada tag ou no "corpo" de toda a plataforma.
Exemplo de propriedade de toda plataforma:
```
* {
    background: blue;
}
```

Para estilização de elementos especificos do HTML, como por exemplo um parágrafo, você pode escolher a **TAG** (**p**) e adicionar a propriedade:
```
p {
  color: blue;
  font-size: 16px;
  font-weight: bold;
}
```

**3. Valor**: O conteúdo atribuído a uma propriedade de estilo específica utilizada dentro do seletor, como `red`, `16px`, `10px, 20px`, etc.

**4. Classe**: Lembra que no artigo de HTML acima, definimos o que é uma classe e ela se chama "destaque"? 
Para poder estilizar a classe HTML no CSS é necessário chama-la e para isso utiliza-se a sintaxe:
```
 .destaque {
     
 }
 ```
 
**5. ID**: Um ID CSS é um seletor que permite aplicar um conjunto específico de regras de estilo a um único elemento HTML, sendo possível deixar ainda mais personalizado ou em destaque.
Caso você queira estilizar a id destaque, no seu código HTML ela vai estar escrita da forma abaixo:
```
<p id="destaque">Este parágrafo possui o ID "destaque".</p>
``` 
E no CSS para estilização vai chamar sua **id** conforme o exemplo:
```
#destaque {
  color: blue;
  font-weight: bold;
}
```
Neste exemplo, o ID "destaque" é atribuído ao primeiro parágrafo usando o atributo id. Em seguida, no CSS, definimos os estilos para o ID #destaque, definindo a cor do texto como azul e o peso da fonte como negrito.

**Faça um teste, copie e cole esse código na sua plataforma**

**6. Pseudoclasse**: Um seletor que seleciona um estado específico de um elemento HTML, como `:hover`, `:active`, `:focus`, etc.
Vamos supor que sua plataforma tem um botão que você deseja chamar atenção, é só aplicar a pseudoclasse **hover**.
Exemplo de código no **HTML**:
```
<button>Hover me!</button>
```
Estilize o botão no **CSS**:
```
button:hover {
  background-color: yellow;
}
```
Desta forma, definimos a cor de fundo do botão como amarelo quando o mouse estiver sobre ele. 
Ou seja, quando o usuário passar o mouse sobre o botão, o fundo do botão mudará para a cor amarela.

**7. Pseudo-elemento**: Um seletor que seleciona partes específicas de um elemento HTML, como `::before`, `::after`, `::first-line`, etc.
Os pseudoelementos, como ::before e ::after, permitem adicionar conteúdo ou estilizar partes específicas dos elementos sem precisar modificar o HTML diretamente.
Eles oferecem maior flexibilidade e controle na manipulação e estilização de elementos na página e possibilita a prática do code clean.
Ex: 
```
.destaque::before {
  content: "Antes: ";
  font-weight: bold;
}
```
O resultado será que o texto "Antes: " será exibido antes do conteúdo do parágrafo, estilizado com o peso da fonte em negrito.


Esses são apenas alguns dos termos básicos utilizados no HTML e CSS. À medida que vamos avançando em nosso aprendizado, você encontrará muitos outros termos e conceitos interessantes.

Tem alguma dica que deseja adicionar? É só comentar e vamos aprendendo juntes.

