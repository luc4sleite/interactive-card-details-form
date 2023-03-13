# Interactive card details form

Esta é uma solução para o desafio do [Interactive card details form challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/interactive-card-details-form-XpS8cKZDWw). 

## Índice

- [Visão geral](#visão-geral)
  - [O desafio](#o-desafio)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [Meu processo](#meu-processo)
  - [Construído com](#construído-com)
  - [O que eu aprendi](#o-que-eu-aprendi)
  - [Desenvolvimento contínuo](#desenvolvimento-contínuo)
  - [Recursos úteis](#recursos-úteis)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

## Visão geral

### O desafio

Os usuários poderão:

- Preencher o formulário e verificar os dados atualizados no cartão
- Receber mensagens de erro quando for submetido no formulário:
  - Campos vazios 
  - O nome do titular, o número do cartão, a data de validade ou o CVC em formatos inválidos
- Visualizar o layout de acordo com o aparelho que estiver utilizando
- Ver as mudanças de estilos conforme interage com a página

### Screenshot

![](./screenshot.jpg)

Add a screenshot of your solution. The easiest way to do this is to use Firefox to view your project, right-click the page and select "Take a Screenshot". You can choose either a full-height screenshot or a cropped one based on how long the page is. If it's very long, it might be best to crop it.

Alternatively, you can use a tool like [FireShot](https://getfireshot.com/) to take the screenshot. FireShot has a free option, so you don't need to purchase it. 

Then crop/optimize/edit your image however you like, add it to your project, and update the file path in the image above.

**Note: Delete this note and the paragraphs above when you add your screenshot. If you prefer not to add a screenshot, feel free to remove this entire section.**

### Links

- Solution URL: [https://www.frontendmentor.io/solutions/formulrio-para-carto-detalhado-interativo-sqV_m4LWgJ](https://www.frontendmentor.io/solutions/formulrio-para-carto-detalhado-interativo-sqV_m4LWgJ)
- Live Site URL: [https://interactive-card-details-form-bice-one.vercel.app](https://interactive-card-details-form-bice-one.vercel.app)

## Meu processo

### Construído com

- Tags HTML5 semânticas
- CSS media queries
- Flexbox
- Mobile-first workflow
- JavaScript

### O que eu aprendi

No projeto eu aprendi a utilizar o JavaScript, através da criação de funções, para identificar e comparar o valor inserido pelo usuário com os formatos que cada campo deveria aceitar

Para isso, utilizei expressões regulares para delimitar o que seria aceito no campo de input, como exemplo para o campo de nome, o input deveria aceitar apenas caracteres e o espaço:

```js
if (inputs[0].value.match(/^[A-Za-z\s]+$/)) {
  cardName.innerHTML = cardHolderName.value;
  inputs[0].style.borderColor = "hsl(270, 3%, 87%)";
  nameError.style.display = "none";
  return true;
} else {
  cardName.innerHTML;
  inputs[0].style.borderColor = "red";
  nameError.style.display = "flex";
  return false;
}
```

### Desenvolvimento contínuo

Devo ampliar meus conhecimentos em JavaScript para que a página possa ser inteira modificada apenas por meio da DOM.
