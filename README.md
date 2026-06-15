# Busca de Cartas Magic

## Descrição
Aplicativo Android que permite aos usuários buscar cartas do jogo Magic: The Gathering. O app oferece filtros por nome, identidade de cor e tipos de carta (Terrenos básicos e Criaturas), exibindo os detalhes principais e a arte da carta na interface.

## API utilizada
- Nome da API: Scryfall API
- Endpoint utilizado: `/cards/random`
- Exemplo de URL consultada: `https://api.scryfall.com/cards/random?q=id:g t:creature`
- Principais dados retornados: Nome da carta, custo de mana, linha de tipo e URIs das imagens.

## Funcionalidades
- Entrada de dados pelo usuário (Spinner e campo de texto)
- Validação de campo vazio (Impede a requisição caso não haja filtro selecionado)
- Consulta de uma API pública
- Exibição dos dados retornados, incluindo carregamento dinâmico de imagem externa
- Tratamento básico de erro (Feedback para o usuário em caso de Erro 404 ou falha de conexão)

## Tecnologias utilizadas
- Kotlin
- Android Studio
- XML
- Biblioteca de requisição utilizada: Volley (para JSON) e Picasso (para imagens)
- API pública escolhida: Scryfall

## Permissões utilizadas
O aplicativo utiliza a permissão INTERNET para realizar requisições à API pública.
````xml
<uses-permission android:name="android.permission.INTERNET" />
````

Como executar o projeto
Clonar este repositório.

Abrir o projeto no Android Studio.

Aguardar a sincronização do Gradle.

Executar o app em um emulador ou dispositivo físico.

Informar um dado válido e realizar a consulta.

Prints do aplicativo:

Tela inicial:

<img width="384" height="808" alt="image" src="https://github.com/user-attachments/assets/3a7c19e0-b2ff-4a92-a43d-d2e473940c9e" />

Resultado da pesquisa:

<img width="385" height="787" alt="image" src="https://github.com/user-attachments/assets/6b91e574-aea2-444b-bbcc-bd21be2e6ef5" />

Autor:

Dyogo Antonio Silva Oliveira
