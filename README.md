
<img alt="GoStack" src="https://storage.googleapis.com/golden-wind/bootcamp-gostack/header-desafios-new.png" />

<h3 align="center">
  Desafio 11: GoRestaurant Mobile
</h3>

## :rocket: Sobre o desafio

O GoRestaurant mobile é a versão para dispositivos móveis dos clientes criada utilizando React Native. Ela se conecta a uma Fake API e exibe e filtra os pratos de comida da API, além de permitir a criação de novos pedidos.

## :warning: Utilizando uma fake API

Antes de tudo, para que você tenha os dados para exibir em tela, criamos um arquivo que você poderá utilizar como fake API para te prover esses dados.

Para isso, deixamos instalado no seu package.json uma dependência chamada `json-server`, e um arquivo chamado `server.json` que contém os dados para as seguintes rotas:

**Rota `/foods`**: Retorna todas as comidas cadastradas na API

**Rota `/foods/:id`**: Retorna um prato de comida cadastradas na API baseado no `id`

**Rota `/categories`**: Retorna todas as categorias cadastradas na API

**Rota `/orders`**: Retorna todas os pedidos que foram cadastrados na API

**Rota `/favorites`**: Retorna todas as comidas favoritas que foram cadastrados na API

```js
  yarn json-server server.json -p 3333
```

## :trophy: Funcionalidades da aplicação

- **`Listar os pratos de comida da sua API`**: A página `Dashboard` é capaz de exibir uma listagem com os campos `name`, `value` e  `description` de todos os pratos de comida que estão cadastrados na sua API.

- **`Listar as categorias da sua API`**: A página `Dashboard` é capaz de exibir uma listagem com os campos `title` e `image_url` de todas as categorias que estão cadastrados na sua API.

- **`Filtrar pratos de comida por busca ou por categorias`**: A página Dashboard permite que o input de pesquisa e os botões de categoria façam uma busca na API de acordo com o que estiver selecionado ou escrito no input.

- **`Listar os pedidos da sua API`**: A página `Orders` é capaz de exibir uma listagem com as informações do produto pedido, com `name` e `description` de todos os pedidos que estão cadastrados na sua API.

- **`Listar os pratos favoritos da sua API`**: A página `Favorites` é capaz de exibir uma listagem com as informações do produto favorito, com `name` e `description` de todos os produtos que estão cadastrados como favoritos na sua API.

- **`Realizar um pedido`**: Na página `Dashboard`, ao clicar em um item, você é direcionado para a página `FoodDetails`, onde é possível realizar um novo pedido, podendo controlar a quantidade desse item pedido, ou adicionar ingredientes extras. Todo o valor é calculado de acordo com a quantidade pedida.

## :computer: Instruções de instalação e teste

Clone o repositório usando o `git` ou faça o download no formato zip. 
Antes de tudo, certifique-se de que você tem um gerenciador de pacotes (como o yarn) e o `Node.js` instalados em sua máquina.

Após baixar o projeto, abra uma aba do terminal e execute os seguintes comandos:

```Bash
# ../pasta-de-destino
$ cd gostack-gorestaurant-mobile
# ../pasta-de-destino/gostack-gorestaurant-mobile
$ yarn
```

Caso esteja usando macOS e vá rodar o app no iOS Simulator ou em um iPhone:

```Bash
# ../pasta-de-destino/gostack-gorestaurant-mobile
$ cd ios
# ../pasta-de-destino/gostack-gorestaurant-mobile/ios
$ pod install
```

Para iniciar a aplicação no iOS:

```Bash
# ../pasta-de-destino/gostack-gorestaurant-mobile
$ yarn ios
```

Para iniciar a aplicação no Android:

```Bash
# ../pasta-de-destino/gostack-gorestaurant-mobile
$ yarn android
```

Para rodar os testes da aplicação:

```Bash
# ../pasta-de-destino/gostack-gorestaurant-mobile
$ yarn test
```
