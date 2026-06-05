# Caso de Teste 3 - Pesquisa de CEP Inexistente

| Campo | Descrição |
|---------|---------|
| **ID** | CT-ViaCep-003 |
| **Título** | Pesquisar CEP Inexistente |
| **Pré-condição** | Usuário acessar o site https://viacep.com.br |

## Passos

1. Acessar o site:
   ```
   https://viacep.com.br
   ```

2. Informar a URL:
   ```
   https://viacep.com.br/ws/99999999/json/
   ```

3. Pesquisar pelo CEP **99999999** (CEP inexistente).

4. Clicar em **Enter**.

## Resultado Esperado

- A API deve retornar uma resposta indicando que o CEP não foi encontrado.
- O retorno deve conter:

   ```json
   {
     "erro": true
   }
   ```

- Status Code **404**.

## Resultado Obtido

- Retorno:

   ```json
   {
     "erro": true
   }
   ```

- Status 404.

