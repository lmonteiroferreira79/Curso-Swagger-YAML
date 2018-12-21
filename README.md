# Swagger II - aula 5 - Customizando a operação consultaExtrato com POSTMAN

## Video 5.1 - Testando a operação consultaExtrato
 
**Iniciar a API**

Startar a API em modo debug.

**Acessar a classe ExtratoApiController.java**

Colocar um breakpoint na operação consultaExtrato

**Acessar a documentação interativa**

http://localhost:8085/bytebank-api/v1/swagger-ui.html 

**Expandir a tag e a operação GET**

Ver os parâmetros necessários para chamar a operação

- As informações da conta no path sendo (agencia, numero e digito) 
- O Authorization no HEADER


**Criar nova request no POSTMAN**

- Método: GET
- URL: http://localhost:8085/bytebank-api/v1/extrato/8756/4/0 


- HEADERS:
```
 Content-Type: application/json
 Authorization: Basic MDEyMzQ1Njc4MzA6c2VuaGExMjM=
```

Lembrando que as informações sobre a conta são aqueles que guardamos após o cadastro do cliente.

Pressionar SEND.

**Resposta da requisição**

Retornou o esperado 501 Not Implemented!

A seguir vamos resolver isso customizando essa operação.
Até já!
