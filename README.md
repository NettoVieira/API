# API, REST e RESTFUL


  <H2>O que é uma API?</H2>

                DE FORMA EXEMPLAR

Cliente(Faz o pedido) - (Client ou pagina na web ou celular)

Garçon(levar seus pedidos, para a a cozinha)(API - "é quem pega os pedidos e leva para o nosso server".)

Cozinha(Server)

            OU NO CONCEITO DA PALAVRA       

Acronimo de Application Programming Interface (Interface de programação de Aplicações) é basicamente um conjunto de rotinas e padrões estabelecidos por uma aplicação, para que outras aplicações possam utilizar as funcionalidades desta aplicação.

        ENTÃO A GENTE PODE ENTENDER QUE A API É


- Responsável por estabelecer comunicação entre diferentes serviços.

- Meio de campo entre as tecnologias.

- Intermediador para troca de informações



# REST

                  DE FORMA EXEMPLAR

<H3>Chegando no restaurante o que você quer? Que o restaurante esteja</H3> 

- limpinho
- Que atenda bem
- Que te atenda bem
- Te dê aquilo que você pediu

<H3>Da mesma forma você, como cliente, não pode chegar no restaurante</H3> 

- Gritando
- Xingando

Mas do que estamos falando aqui? Estamos tratando sobre boas praticas. Temos que ter algo para respeitar,para que tudo possa ocorrer legal! 

<h3> o Rest é isso!!</h3>

Ele determina algumas obrigações nessa transferência de dados!


              OU NO CONCEITO DA PALAVRA


Um acrônimo para Representational State Transfer (Transferência de Estado Representativo)

Sera feita a transferência de dados de uma maneira simbólica, de maneira mais didática e geralmente são feitas tais transferências utilizando o protocolo HTTP.

Alem de demilimitar algumas obrigações nessas transferências de Dados

Os dados no rest nós vamos chama-lo de 'Resources', uma entidade ou um objeto.

<h3>Como dado no exemplo acima na parte de API</h3>

Nós sabemos que o cliente fará um pedido e o garçon anotara o pedido em um bloco de notas, e levara até a cozinha para passar qual foi o pedido do cliente, logo sabemos que, o bloco de notas do garçom é a nossa transferência de Dados com o protocolo HTTP.

# 6 NECESSIDADES(constraints) para ser RESTful

- _Cliente-server_ : Separação do cliente e do armazenamento de dados (servidor), dessa forma, poderemos ter uma portabilidade do nosso sistema, usando o React para WEB e React Native para o smartphone, por exemplo.

- _stateless_: Cada requisição que o cliente faz para o servidor, deverá conter todas as informações necessárias para o servidor entender e responder (RESPONSE) a requisição (REQUEST). Exemplo: A sessão do usuário deverá ser enviada em todas as requisições, para saber se aquele usuário está autenticado e apto a usar os serviços, e o servidor não pode lembrar que o cliente foi autenticado na requisição anterior. Existem alguns padrões como o de usar Tokens para a comunicação.

- _Cacheable_: As respostas para a uma requisição, deverão ser explicitas ao dizer se aquela requisição, pode ou não ser cacheada pelo cliente.

- _Uniform Interface_: É, basicamente, um contrato para comunicação entre clientes e servidor. São pequenas regras para deixar um componente o mais genérico possível, o tornando muito mais fácil de ser refatorado e melhorado.

- _Layered System_: O cliente acessa a um endpoint, sem precisar saber da complexidade, de quais passos estão sendo necessários para o servidor responder a requsição, ou quais outras camadas o servidor estará lidando, para que a requsição seja respondida.

- _code on demand (optional)_: Dá a possibildiade da nossa aplicação pegar códigos, como o javascript, por exemplo, e executar no cliente.

# RESTFUL
RESTful, é a aplicação dos padrões REST.

# BOAS PRATICAS
- Utilzar verbos HTTP para nossas requisições
- Utilizar plural ou singular na criação dos endpoints? _NÃO IMPORTA!_ use um padrão!
- Não deixar barra no final do endpoint
- Nunca deixa o cliente sem resposta

## Verbos HTTP
- GET: Receber dados de um resource
- POST: Enviar dados ou informaçõe sde resource
- PUT: Atualizar dados de um resource
- DELETE: deletar um resource


# STATUS DAS RESPOSTAS
- 1xx: Informação

- 2xx: Sucesso
 - 200: OK
 - 201: CREATER
 - 204: Não tem conteúdo PUT POST DELETE

- 3xx: Redirection

- 4xx: Client Error
 - 400: Bad Request
 - 404: Not Found

- 5xx: Server Error
 - 500: Internal Server Error


