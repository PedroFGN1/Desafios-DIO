# Sistema Bancário com Funções Python

Este é um projeto de um sistema bancário simples desenvolvido em Python, otimizado com o uso de funções. O programa permite realizar operações bancárias básicas como depósitos, saques, visualização de extrato, criação de usuários e contas, e listagem de contas.

## Funcionalidades

- **Depositar**: Permite depositar um valor positivo na conta.
- **Sacar**: Permite sacar um valor, com limite de R$ 500 por saque e no máximo 3 saques por dia.
- **Extrato**: Exibe o histórico de transações e o saldo atual.
- **Novo Usuário**: Cria um novo usuário com CPF, nome, data de nascimento e endereço.
- **Nova Conta**: Cria uma nova conta corrente vinculada a um usuário existente.
- **Listar Contas**: Lista todas as contas criadas com seus detalhes.
- **Sair**: Encerra o programa.

## Requisitos

- Python 3.x instalado no sistema.

## Como Executar

1. Certifique-se de que o Python está instalado.
2. Navegue até a pasta do projeto: `Otimizando o Sistema Bancário com Funções Python`.
3. Execute o arquivo `desafio.py` com o comando:
   ```
   python desafio.py
   ```
4. Siga as instruções no menu interativo.

## Estrutura do Código

- `menu()`: Exibe o menu de opções e retorna a escolha do usuário.
- `depositar(saldo, valor, extrato, /)`: Função para depósito, recebe argumentos apenas por posição.
- `sacar(*, saldo, valor, extrato, limite, numero_saques, limite_saques)`: Função para saque, recebe argumentos apenas por nome.
- `exibir_extrato(saldo, /, *, extrato)`: Exibe o extrato, com saldo posicional e extrato nomeado.
- `criar_usuario(usuarios)`: Cria um novo usuário e adiciona à lista.
- `filtrar_usuario(cpf, usuarios)`: Filtra usuários por CPF.
- `criar_conta(agencia, numero_conta, usuarios)`: Cria uma nova conta para um usuário.
- `listar_contas(contas)`: Lista todas as contas criadas.
- `main()`: Função principal que controla o fluxo do programa.

## Limitações

- Dados são armazenados apenas em memória (não persistem após o fechamento do programa).
- Não há autenticação de usuários.
- Limite de saques: 3 por dia, R$ 500 por saque.

## Autor

Desenvolvido como parte de um desafio da DIO.