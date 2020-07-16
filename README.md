## Aprendendo GraphQL

### Desafio 02 Front-end

Este é um pequeno projeto front-end desenvolvido com Vue.js. Ele é responsável por consumir a API desenvolvida do Desafio 02.

#### 💻 Ambiente

Aplicação inicializada com o _boilerplate_ (`vue create <nome_do_projeto>`) oficial do Vue.js. Para execução deste projeto, não se faz necessário, apenas o Node.js e NPM. No entanto, caso queira incializar o próprio projeto baseado no _boilerplate_, é preciso que o Vue CLI (`@vue/cli`) esteja instalado na máquina.

#### 📚 Libs

As bibliotecas listadas abaixo são terceiras ao Vue.js, as bibliotecas "nativas" desse ecossistema estão inclusas, porém não são mencionadas aqui.

1. **apollo-cache-inmemory** para amarzenamento em _cache_ das requisições na memória do navegador (apenas tempo de execução)
1. **apollo-client** para a realização de requisições para APIs GQL. O Apollo Client é voltado para o _client-side_ da aplicação
1. **apollo-link-context** para a injeção do token JWT de autentição em cada requisição feita
1. **apollo-link-http** para concatenação do contexto com o _end-point_ da API
1. **graphql** para manipulação de requisições GQL
1. **graphql-tag** para "parseamento" (conversão) das _strings_ no formato GQL em objetos JS para manipulação das requisições
1. **vuetify** para estilização e dinâmica da aplicação. Oferece uma série de componentes bem definidos baseados no [Material Design](https://material.io/design).

#### ⚙️ Configuração e execução do projeto

Abaixo segue um subjunto de comando possíveis de serem executados com Vue.js.

###### Configuração incial

```
npm install
```

###### Compilação e _hot-reloads_ para desenvolvimento

```
npm run serve
```

###### Compilação e minificados para produção

```
npm run build
```
