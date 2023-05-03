# Documentação do projeto "Criando Extensão de Favoritos para o Google Chrome com JavaScript"

Esta é uma extensão simples do Google Chrome que permite ao usuário salvar seus favoritos em uma lista local. O usuário pode adicionar favoritos clicando no botão "Adicionar aos favoritos", que salva o título da página e sua URL na lista local. A lista de favoritos pode ser visualizada clicando no ícone da extensão no canto superior direito da tela.

O vídeo que criei para ajudar [Clique aqui](https://youtu.be/SFetypYCsX4)


## Como usar
1. Faça o download dos arquivos do projeto.
2. Abra o Google Chrome e vá para a página chrome://extensions.
3. Ative o "Modo do desenvolvedor" no canto superior direito da tela.
4. Clique em "Carregar sem compactação" e selecione a pasta do projeto.
5. A extensão será adicionada ao Google Chrome e um ícone será exibido no canto superior direito da tela.
6. Clique no ícone da extensão para visualizar a lista de favoritos.
7. Clique no botão "Adicionar aos favoritos" na página que você deseja salvar.
8. O título da página e sua URL serão adicionados à lista de favoritos.

## Arquivos
O projeto é composto por três arquivos:

- `index.html`: contém a estrutura HTML da página da extensão.
- `style.css`: contém o estilo CSS da página da extensão.
- `script.js`: contém o código JavaScript que salva e carrega os favoritos.

## Como funciona
O código JavaScript da extensão utiliza a API `chrome.tabs` para obter informações sobre a página ativa, como sua URL e título. Quando o usuário clica no botão "Adicionar aos favoritos", o título da página e sua URL são salvos em um objeto e adicionados a um array de objetos que é armazenado na lista local de armazenamento do navegador usando a API `localStorage`. Quando a página da extensão é carregada, o array é recuperado da lista local de armazenamento e cada objeto é renderizado na página como um item de lista.
