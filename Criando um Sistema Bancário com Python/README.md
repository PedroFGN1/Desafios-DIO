# Sistema Bancário em Python

Este é um projeto simples de um sistema bancário desenvolvido em Python, como parte de um desafio de programação. O objetivo é implementar operações básicas de um banco, como depósito, saque e visualização de extrato, utilizando apenas variáveis e estruturas de controle.

## Descrição do Projeto

O sistema permite ao usuário realizar as seguintes operações:

- **Depósito**: Permite depositar valores positivos na conta bancária. Todos os depósitos são armazenados e exibidos no extrato.
- **Saque**: Permite realizar até 3 saques diários, com limite máximo de R$ 500,00 por saque. Verifica se há saldo suficiente e se o limite de saques não foi excedido.
- **Extrato**: Exibe todas as movimentações realizadas (depósitos e saques) e o saldo atual da conta, formatado em reais (R$ xxx.xx).

O projeto trabalha com apenas 1 usuário, sem necessidade de identificar agência ou conta bancária.

## Funcionalidades Implementadas

- **Menu Interativo**: Um menu simples em loop que permite ao usuário escolher entre as operações.
- **Validação de Entradas**: Verificações para valores positivos, saldo suficiente, limites de saque e número máximo de saques.
- **Armazenamento de Dados**: Uso de variáveis para saldo, extrato e contador de saques.
- **Formatação de Valores**: Valores exibidos no formato brasileiro (R$ xxx.xx).

## Estrutura do Código

O código principal está no arquivo `desafio.py`, que contém:

- Variáveis globais: `saldo`, `limite`, `extrato`, `numero_saques`, `LIMITE_SAQUES`.
- Um loop infinito com menu de opções.
- Condicionais para cada operação: depósito, saque, extrato e sair.

## Como Executar

1. Certifique-se de ter Python instalado (versão 3.x).
2. Execute o arquivo `desafio.py` no terminal:
   ```
   python desafio.py
   ```
3. Siga as instruções no menu para realizar as operações.

## Exemplo de Uso

- Escolha "d" para depositar um valor.
- Escolha "s" para sacar (até 3 vezes por dia, máximo R$ 500).
- Escolha "e" para ver o extrato.
- Escolha "q" para sair.

## Considerações Finais

Este projeto é uma versão básica (v1) e serve como exercício de programação. Futuras versões poderiam incluir múltiplos usuários, persistência de dados em arquivos ou banco de dados, e mais funcionalidades como transferências.
