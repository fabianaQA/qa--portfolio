# CT-ViaCep-001 - Pesquisar CEP

## Objetivo
Validar a consulta de um CEP utilizando a API ViaCEP e verificar se o retorno ocorre com status code 200 e com os dados corretos do endereço pesquisado.

## Pré-condições
- Usuário com acesso à internet.
- Navegador disponível.

## Dados de Teste

| Campo | Valor |
|---------|---------|
| CEP | 01001000 |
| URL | https://viacep.com.br/ws/01001000/json/ |

## Passos para Execução

1. Acessar o site https://viacep.com.br

2. Informar a URL:
   `https://viacep.com.br/ws/01001000/json/`

3. Pressionar **Enter**.

4. Validar o retorno da consulta.

## Resultado Esperado

- A requisição deve retornar **Status Code 200**.
- O retorno deve estar no formato **JSON**.
- Os campos do CEP devem ser retornados de acordo com a pesquisa realizada.

### Campos Esperados

| Campo | Valor Esperado |
|---------|----------------|
| cep | 01001-000 |
| logradouro | Praça da Sé |
| complemento | lado ímpar |
| bairro | Sé |
| localidade | São Paulo |
| uf | SP |
| estado | São Paulo |
| regiao | Sudeste |
| ibge | 3550308 |
| gia | 1004 |
| ddd | 11 |
| siafi | 7107 |

## Critério de Sucesso

- Status HTTP igual a **200**.
- Todos os campos retornados correspondem ao CEP pesquisado.
- Não deve existir o campo `"erro": true` na resposta.

## Resultado Esperado Final

**Status 200 com os campos corretos retornados para o CEP pesquisado.**

Observação: o CEP 01001000 não corresponde à Rua Santa Fé. Ele retorna a Praça da Sé - São Paulo/SP. Se o teste deve validar a Rua Santa Fé, será necessário utilizar o CEP correto dessa rua.
