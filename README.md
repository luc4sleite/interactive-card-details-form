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

![Screenshot 2023-03-12 at 22-06-18 Formulário para cartão de crédito](https://user-images.githubusercontent.com/115735167/224586329-5d9d3411-9eb9-4afe-ada6-4c008fd23207.png)
![Screenshot 2023-03-12 at 22-06-54 Formulário para cartão de crédito](https://user-images.githubusercontent.com/115735167/224586356-67a2d667-3e92-46b8-a0d2-18825f2f37a6.png)
![Screenshot 2023-03-12 at 22-07-33 Formulário para cartão de crédito](https://user-images.githubusercontent.com/115735167/224586390-bd0ee7e8-0abd-4189-af19-fec7dbc54d47.png)
![Screenshot 2023-03-12 at 22-07-59 Formulário para cartão de crédito](https://user-images.githubusercontent.com/115735167/224586422-b0f6c324-3d2d-4ae1-92d9-f0425a8ab22c.png)



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
