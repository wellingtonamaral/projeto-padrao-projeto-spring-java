# Explorando Padrões de Projetos na Prática com Java

Repositório com as implementações dos padrões de projeto explorados no Lab "Explorando Padrões de Projetos na Prática com Java". 

Especificamente, este projeto explorou alguns padrões usando o Spring Framework, são eles:

- Singleton
- Strategy/Repository
- Facade

Esse projeto é uma API REST que recupera os dados do cep informado.

É possivel visualizar os a documentação do ViaCep, webservice gratuito [aqui](https://viacep.com.br/).

Exemplo de entrada usando método POST:
```json
{
  "id": 1,
  "nome": "Wellington Amaral",
  "endereco": {
    "cep": "24110400"
  }
}
```
Saída:

```json
{
  "id": 1,
  "nome": "Wellington Amaral",
  "endereco": {
    "cep": "24110-400",
    "logradouro": "Rua Amerino Vanick",
    "complemento": "",
    "bairro": "Barreto",
    "localidade": "Niterói",
    "uf": "RJ",
    "ibge": "3303302",
    "gia": "",
    "ddd": "21",
    "siafi": "5865"
  }
}
```

Testar os dados do JSON:
```
    localhost:8080/swagger-ui.html
  ou
    127.0.0.1:8080/swagger-ui.html
```
![swagger](https://github.com/wellingtonamaral/projeto-padrao-projeto-spring-java/assets/31280586/95da6b81-76c9-40cd-9de5-f16fa12117ba)
