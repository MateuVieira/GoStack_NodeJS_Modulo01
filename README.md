# GoStack Rocketseat 🚀

Nesse repositório vou armazenar todas as minhas anotações, códigos e exercícios feitos durante o bootcamp GoStack 10 da Rocketseat referente ao modulo 01.

## Módulo 01 - Conceitos

### Dependências

-   Express
-   Nodemon

### Inicializar

-   yarn dev

### Conteúdo da Requisição

Com o node, temos acesso a 3 tipos de fontes de dados enviados por meio de requisição.

-   Query Params
-   Route Params
-   Body Params
-   (Adicional) Headers

### Query Params

Nos parâmetros obtidos pela Query, podemos enviar dados de pesquisa, como o id do usuário ou do produto que desejamos pesquisar ou editar. Esses dados serão inseridos na URL da requisição, sendo assim, é necessário utilizar esses parâmetros com sabedoria, pois não podemos inserir dados sigilosos nesse tipo de requisição. Exemplo: **/page?number=2**

### Route Params

Nos parâmetros de rotas, podemos enviar também dados de pesquisa. Como esse tipo de parâmetro também vai ser enviado pela URL, tem muitas características que também se encontra no _Query Params_. Porém nesse tipo de requisição, os dados são enviados de uma forma _friendly user_. Exemplo: **/page/2/**

### Body Params

Pelo contrário aos outros, esse método de envio de dados na requisição é mais seguro, pois é significativamente mais difícil expor esses dados a usuários. Esses dados são enviados juntamente com a requisição e não precisam ser expostos na URL. Deve ser usado principalmente em duas ocasiões:

1.  Não expor os dados durante o envio
2.  Possibilidade de anexar maior quantidade de dados

### Headers

São dados que normalmente não se repetem e que complementam a requisição como: Com que tipo de estrutura as informações estão sendo enviadas, qual é o tipo de estrutura que a resposta precisa ter, informações de acesso como token, locations, languages, etc.

### Http Codes

Os **HTTP CODES** são números que são enviados na resposta de cada requisição. Elas têm a finalidade de explicar o resultado do back-end em relação a requisição. Existem diversos **HTTP Codes**:

-   1xx - Informational
-   2xx - Success
    -   200 - OK: Tudo deu certo!
    -   201 - CREATED: Conteúdo foi criado com sucesso!
-   3xx - Redirection
    -   301 - MOVED PERMANENTLY: A página foi mudada para outra URL permanentemente.
    -   302 - MOVED: A página foi movida.
-   4xx - Client Error
    -   400 - BAD REQUEST: Erro nos parâmetros enviados.
    -   401 - UNAUTHORIZED: Usuário não autorizado para executar essa ação.
    -   404 - NOT FOUND: Conteúdo não encontrado
-   5xx - Server Error
    -   500 - INTERNAL SERVER ERROR: Erro interno do servidor. (Precisa de tratamento no back-end mas também pode ser encarado como erro nos parâmetros)
    
    
