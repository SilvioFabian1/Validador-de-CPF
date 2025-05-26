# Validador de CPF em JavaScript

Este projeto implementa uma classe chamada `VerificaCPF` para validar números de CPF (Cadastro de Pessoa Física) no formato brasileiro. A validação segue as regras oficiais de cálculo dos dígitos verificadores.

## 📋 Como funciona

A classe `VerificaCPF` executa as seguintes etapas:

1. **Limpeza do CPF:** Remove caracteres como pontos, traços e espaços, retornando apenas os 11 dígitos.
2. **Validação de repetição:** Impede que CPFs compostos por dígitos repetidos (como `111.111.111-11`) sejam considerados válidos.
3. **Cálculo dos dígitos verificadores:** Verifica se os dois últimos dígitos do CPF correspondem aos valores esperados, conforme o algoritmo de validação.

## 🚀 Exemplo de uso

```js
const cpf = new VerificaCPF('123.456.789-09');
cpf.init(); // CPF Inválido
