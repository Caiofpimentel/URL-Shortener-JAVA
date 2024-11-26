# URL Shortener Service

🌐 Como Funciona?

Requisição para criação de URL encurtada: 
Faça uma requisição HTTP POST para o endpoint:

https://wnuvaq8gjj.execute-api.sa-east-1.amazonaws.com/create
Corpo da requisição (JSON):
{
    "expirationTime": "TimeStamp em milissegundos",
    "originalUrl": "https://exemplo.com/"
}

Resposta da API:
A API retornará um identificador único (UUID) no seguinte formato:

json
{
    "code": "8d1e2f34"
}

Acessando a URL encurtada:
Anexe o código retornado ao final da URL base para acessar o link original:

https://wnuvaq8gjj.execute-api.sa-east-1.amazonaws.com/8d1e2f34

Ao acessar o link encurtado, você será redirecionado para a URL original configurada na requisição.


## 🚀 Tecnologias Utilizadas

- **Java 17**: Linguagem principal da aplicação.
- **Amazon API Gateway**: Para expor as APIs REST.
- **AWS Lambda**: Para execução de funções serverless.
- **Amazon S3**: Para armazenamento das URLs encurtadas e originais.

---
