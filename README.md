# Card Pix

Bem-vindo ao repositório do projeto "Card Pix". Este repositório contém um exemplo de uma página HTML e CSS que exibe um cartão estilizado para transferências via Pix, com efeitos visuais ao passar o mouse sobre o cartão.

## Visão Geral

O projeto consiste em uma página web simples que utiliza HTML e CSS para criar um cartão interativo. O objetivo é demonstrar como aplicar estilos CSS para modificar a aparência de elementos ao passar o mouse sobre eles (hover effect).

## Estrutura do Projeto

A estrutura do projeto é composta por um arquivo HTML com estilos embutidos. Aqui está um resumo da estrutura do código:

- **HTML**: Define a estrutura básica da página e do cartão.
- **CSS**: Estilos embutidos no HTML para layout e efeitos de hover.

## Arquivo Principal

### index.html

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Card Pix</title>

    <style>
      * {
        margin: 0;
        padding: 0;
        box-sizing: border-box;
        font-family: Arial, Helvetica, sans-serif;
      }

      .container {
        position: relative;
        width: 100vw;
        height: 100vh;
        background-color: #d6d4e2;
        display: flex;
        flex-direction: row;
        justify-content: center;
        align-items: center;
      }
      .cardPix {
        width: 208px;
        height: 244px;
        padding: 32px 24px 32px 24px;
        background-color: #ffffff;
        gap: 10px;
        border-radius: 32px;
        cursor: pointer;
      }
      .cardPix:hover {
        color: white;
        background-color: black;
      }
      .cardPix:hover .img {
        opacity: 0;
        display: none;
        background-color: black;
      }
      .cardPix:hover h1 {
        color: white;
      }
      h1 {
        font-weight: 500;
        font-size: 20px;
        line-height: 28px;
        color: #787490;
      }
      span {
        font-size: 22px;
        line-height: 48px;
      }
    </style>
  </head>
  <body>
    <div class="container">
      <div class="cardPix">
        <img class="img" src="/svg/Union.svg" alt="logo" />
        <img class="imgHover" src="/svg/icon-pix.svg" alt="logo" />
        <h1>Transferências via Pix</h1>
        <span>R$150,00</span>
      </div>
    </div>
  </body>
</html>
```

## Instruções

### Requisitos

- Navegador web atualizado

### Execução

1. Clone este repositório:
   ```sh
   git clone https://github.com/seu-usuario/card-pix.git
   ```

2. Navegue até o diretório do projeto:
   ```sh
   cd card-pix
   ```

3. Abra o arquivo `index.html` no seu navegador preferido para visualizar a página.

## Funcionalidades

- **Efeito Hover**: Ao passar o mouse sobre o cartão, ele muda de cor e os elementos internos são alterados para destacar a interação.
- **Estilização Responsiva**: A página utiliza flexbox para centralizar o cartão, garantindo que ele esteja centralizado tanto vertical quanto horizontalmente na tela.

## Contribuição

Contribuições são bem-vindas! Sinta-se à vontade para abrir issues e pull requests.

## Licença

Este projeto está licenciado sob a licença MIT. Veja o arquivo `LICENSE` para mais detalhes.

---

Esperamos que este projeto sirva como um bom exemplo para praticar HTML e CSS. Aproveite e boa codificação!
