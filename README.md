## **Sistema Bancário em Python - Desafio Bootcamp DIO**
Este projeto foi desenvolvido como parte do desafio do bootcamp da DIO. Ele simula um sistema bancário simples utilizando Programação Orientada a Objetos (POO) em Python. A aplicação oferece funcionalidades comuns em um sistema bancário, como depósitos, saques, exibição de extrato, criação de contas e usuários.

![Dashboard](https://thumbs.dreamstime.com/z/desenho-animado-com-ilustra%C3%A7%C3%A3o-de-diferentes-varia%C3%A7%C3%B5es-monet%C3%A1rias-que-ilustra-formas-armazenar-e-economizar-dinheiro-215168940.jpg?w=992)

## **Funcionalidades**

O sistema oferece as seguintes operações:

- **Depositar**: Permite ao usuário realizar depósitos em sua conta.
- **Sacar**: Realiza saques, verificando se o valor é válido e se há saldo suficiente.
- **Exibir Extrato**: Exibe o extrato com todas as movimentações da conta.
- **Nova Conta**: Cria uma nova conta bancária para um usuário existente.
- **Listar Contas**: Exibe todas as contas cadastradas com informações básicas.
- **Novo Usuário**: Cadastra um novo usuário no sistema.
- **Sair**: Encerra a aplicação.

## **Estrutura do Código**

### Funções Principais:

- `menu()`: Exibe o menu principal e captura a opção escolhida pelo usuário.
- `depositar(saldo, valor, extrato)`: Recebe o valor do depósito e atualiza o saldo e o extrato.
- `sacar(saldo, valor, extrato, limite, numero_saques, limite_saques)`: Realiza o saque se o saldo, limite e número máximo de saques permitirem.
- `exibir_extrato(saldo, extrato)`: Exibe todas as movimentações e o saldo atual.
- `criar_usuario(usuarios)`: Adiciona um novo usuário com CPF, nome completo, data de nascimento e endereço.
- `criar_conta(agencia, numero_conta, usuarios)`: Cria uma nova conta vinculada a um usuário existente.
- `listar_contas(contas)`: Exibe todas as contas cadastradas.
- `main()`: Executa o loop principal, gerenciando as interações e chamando as funções apropriadas.

### Regras de Negócio:

- O **limite de saques** diários é configurado como 3.
- O **limite de valor por saque** é de R$ 500,00.
- Depósitos devem ser positivos, e o saldo é atualizado automaticamente.
- Para **criação de conta**, é necessário que o usuário já esteja cadastrado no sistema.
- **Extrato** mostra todas as transações realizadas.
