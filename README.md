# 📈 Checkpoint Crypto

Aplicativo Android desenvolvido em **Kotlin** que consome a API do **Mercado Bitcoin** para exibir informações atualizadas sobre o valor do Bitcoin (BTC).

## 🔧 Tecnologias utilizadas

- Kotlin
- Android SDK
- Retrofit (para chamadas HTTP)


## ⚙️ Funcionalidades

- Busca em tempo real do valor atual do Bitcoin usando a API pública do [Mercado Bitcoin](https://www.mercadobitcoin.net/).
- Exibe o último preço do BTC formatado em reais (R$).
- Mostra a data e hora da última atualização.
- Botão de **"Atualizar"** para realizar novas chamadas e obter os dados mais recentes.
- Layout simples e objetivo, com uso de `Toolbar` personalizada.

## 🧠 Estrutura do Projeto

### `MainActivity.kt`
Tela principal do app. Responsável por:
- Configurar a interface (toolbar, botões e textos).
- Realizar a chamada à API e atualizar os dados na tela.
- Tratar erros de conexão ou falhas na resposta.

### `MercadoBitcoinService.kt`
Interface Retrofit que define o endpoint da API:
- `GET api/BTC/ticker/` → Retorna informações atualizadas sobre o BTC.

### `MercadoBitcoinServiceFactory.kt`
Classe que cria e configura o cliente Retrofit.

### `TickerResponse.kt`
Modelos de dados que representam a resposta da API:
- `TickerResponse` contém um objeto `Ticker`, que possui os dados como preço, volume, data, etc.

## 📲 Como usar

1. Instale o projeto em um dispositivo Android ou emulador.
2. Abra o app e clique em **Atualizar** para ver o valor atual do Bitcoin.
3. Os dados serão exibidos com o preço em real e a data da última atualização.

## 📦 API usada

- [https://www.mercadobitcoin.net/api/BTC/ticker/](https://www.mercadobitcoin.net/api/BTC/ticker/)

---

Desenvolvido para fins acadêmicos por 
- Felipe Cardoso RM 99062
- Carlos Augusto RM 98456


