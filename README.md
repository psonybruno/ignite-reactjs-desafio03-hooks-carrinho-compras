# Desafio 03 - Criando um hook de carrinho de compras
# 💻 Sobre o desafio

Nesse desafio, você deverá criar uma aplicação para treinar o que aprendeu até agora no ReactJS
Essa será uma aplicação onde o seu principal objetivo é criar um hook de carrinho de compras. Você terá acesso a duas páginas, um componente e um hook para implementar as funcionalidades pedidas nesse desafio:

  - Adicionar um novo produto ao carrinho;
  - Remover um produto do carrinho;
  - Alterar a quantidade de um produto no carrinho;
  - Cálculo dos preços sub-total e total do carrinho;
  - Validação de estoque;
  - Exibição de mensagens de erro;
  - Entre outros.

# Se preparando para o desafio
  - Fake API com JSON Server;
    ```
    yarn
    yarn server
    ```
  - Preservar dados do carrinho com localStorage API;
    ```
    localStorage.setItem('@RocketShoes:cart', cart)
    const storagedCart = localStorage.getItem('@RocketShoes:cart');
    ```
  - Mostrar erros com toastify.
    [React Toastify](https://github.com/fkhadra/react-toastify#readme)

## O que devo editar na aplicação?
Com o template já clonado, as depêndencias instaladas e a [fake API rodando](https://www.notion.so/Desafio-01-Criando-um-hook-de-carrinho-de-compras-5769216778794019a83f544e79167b12), você deve completar onde não possui código com o código para atingir os objetivos de cada teste. Os documentos que devem ser editados são:

- **src/components/Header/index.tsx**
- **src/pages/Home/index.tsx**
- **src/pages/Cart/index.tsx**
- **src/hooks/useCart.tsx**

## Especificação dos testes
- Teste components/Header/index.tsx
  - [x] - should be able to render the amount of products added to cart

- Teste pages/Home/index.tsx
  - [x] - should be able to render each product quantity added to cart
  - [x] - should be able to add a product to cart

- Testes pages/Cart/index.tsx
  - [x] - should be able to increase/decrease a product amount
  - [x] - should not be able to decrease a product amount when value is 1
  - [x] - should be able to remove a product

- Testes hooks/useCart.tsx
  - [x] - should be able to initialize cart with localStorage value
  - [x] - should be able to add a new product
  - [x] - should not be able add a product that does not exist
  - [x] - should be able to increase a product amount when adding a product that already exists on cart
  - [x] - should not be able to increase a product amount when running out of stock
  - [x] - should be able to remove a product
  - [x] - should not be able to remove a product that does not exist
  - [x] - should be able to update a product amount
  - [x] - should not be able to update a product that does not exist
  - [x] - should not be able to update a product amount when running out of stock
  - [x] - should not be able to update a product amount to a value smaller than 1