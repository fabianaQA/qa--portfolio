# Caso de Teste 2 - Pesquisa de CEP Inválido

| Campo | Descrição |
|---------|---------|
| **ID** | CT-ViaCep-002 |
| **Título** | Pesquisar CEP Inválido |
| **Pré-condição** | Usuário acessar o site https://viacep.com.br |

## Passos

1. Acessar o site https://viacep.com.br
2. Informar a URL:
   ```
   https://viacep.com.br/ws/abcdef/json/
   ```
3. Pesquisar pelo CEP **abcdef** (CEP inválido).
4. Clicar em **Enter**.

## Resultado Esperado

- Retornar **Status Code 400**.

## Resultado Obtido

- Status 400.
