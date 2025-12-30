# Sistema Bancário em POO com Python

Este é um projeto de um sistema bancário desenvolvido em Python utilizando Programação Orientada a Objetos (POO). O programa modela entidades como clientes, contas, transações e histórico, permitindo operações bancárias básicas de forma estruturada e reutilizável.

## Funcionalidades

- **Depositar**: Permite depositar um valor positivo em uma conta corrente.
- **Sacar**: Permite sacar um valor, com limite de R$ 500 por saque e no máximo 3 saques por dia.
- **Extrato**: Exibe o histórico de transações e o saldo atual da conta.
- **Novo Usuário**: Cria um novo cliente pessoa física com CPF, nome, data de nascimento e endereço.
- **Nova Conta**: Cria uma nova conta corrente vinculada a um cliente existente.
- **Listar Contas**: Lista todas as contas criadas com seus detalhes.
- **Sair**: Encerra o programa.

## Requisitos

- Python 3.x instalado no sistema.

## Como Executar

1. Certifique-se de que o Python está instalado.
2. Navegue até a pasta do projeto: `Modelando o Sistema Bancário em POO com Python`.
3. Execute o arquivo `desafio.py` com o comando:
   ```
   python desafio.py
   ```
4. Siga as instruções no menu interativo.

## Estrutura do Código (Classes e Conceitos de POO)

### Classes Principais

- **Cliente**: Classe base para clientes, com endereço e lista de contas.
  - **PessoaFisica**: Subclasse de Cliente, representa pessoa física com nome, data de nascimento e CPF.

- **Conta**: Classe base para contas bancárias, com saldo, número, agência, cliente e histórico.
  - **ContaCorrente**: Subclasse de Conta, com limite de saque e limite de número de saques.

- **Historico**: Classe para armazenar o histórico de transações de uma conta.

- **Transacao**: Classe abstrata para transações.
  - **Saque**: Subclasse para operações de saque.
  - **Deposito**: Subclasse para operações de depósito.

### Funções de Interface

- `menu()`: Exibe o menu de opções e retorna a escolha do usuário.
- `filtrar_cliente(cpf, clientes)`: Filtra clientes por CPF.
- `recuperar_conta_cliente(cliente)`: Recupera a primeira conta de um cliente.
- `depositar(clientes)`: Realiza depósito para um cliente.
- `sacar(clientes)`: Realiza saque para um cliente.
- `exibir_extrato(clientes)`: Exibe o extrato de um cliente.
- `criar_cliente(clientes)`: Cria um novo cliente.
- `criar_conta(numero_conta, clientes, contas)`: Cria uma nova conta para um cliente.
- `listar_contas(contas)`: Lista todas as contas.
- `main()`: Função principal que controla o fluxo do programa.

## Conceitos de POO Utilizados

- **Herança**: ContaCorrente herda de Conta; PessoaFisica herda de Cliente; Saque e Deposito herdam de Transacao.
- **Encapsulamento**: Atributos privados (prefixo `_`) e propriedades para acesso controlado.
- **Abstração**: Classe Transacao é abstrata, com métodos abstratos.
- **Polimorfismo**: Métodos como `sacar` e `registrar` são sobrescritos nas subclasses.

## Limitações

- Dados são armazenados apenas em memória (não persistem após o fechamento do programa).
- Não há autenticação de usuários.
- Cada cliente pode ter apenas uma conta (a primeira é usada por padrão).
- Limite de saques: 3 por dia, R$ 500 por saque.

## Autor

Desenvolvido como parte de um desafio da DIO.