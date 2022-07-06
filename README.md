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