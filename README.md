# Sistema_bancario_avancado_POO.py

Classes Principais:
Cliente:

Possui um endereço e uma lista de contas associadas a esse cliente.
Métodos para realizar transações e adicionar contas.
PessoaFisica (Herda de Cliente):

Representa uma pessoa física, com atributos como nome, data de nascimento, CPF, e endereço.
Conta:

Representa uma conta bancária básica, com saldo, número, agência, cliente associado, e um histórico de transações.
Métodos para saque, depósito e criação de uma nova conta.
ContaCorrente (Herda de Conta):

Especialização de conta que inclui um limite de saque e controle do número de saques.
Historico:

Mantém um registro de transações associadas a uma conta.
Transacao (Classe Abstrata):

Define a estrutura básica para uma transação, com propriedades e método abstrato para registrar.
Saque (Herda de Transacao):

Representa uma transação de saque.
Deposito (Herda de Transacao):

Representa uma transação de depósito.
Funções Principais:
menu():

Mostra um menu simples para o usuário, permitindo escolher a operação desejada.
filtrar_cliente(cpf, clientes):

Filtra clientes por CPF.
recuperar_conta_cliente(cliente):

Recupera a primeira conta associada a um cliente.
depositar(clientes):

Solicita informações e realiza um depósito para um cliente.
sacar(clientes):

Solicita informações e realiza um saque para um cliente.
exibir_extrato(clientes):

Solicita informações e exibe o extrato de um cliente.
criar_cliente(clientes):

Solicita informações e cria um novo cliente.
criar_conta(numero_conta, clientes, contas):

Solicita informações e cria uma nova conta associada a um cliente.
listar_contas(contas):

Lista todas as contas existentes.
main():

Loop principal do programa, onde o usuário pode interagir com o sistema bancário.
Observações:
A estrutura do código segue o paradigma de orientação a objetos.
São usadas classes e herança para modelar os diferentes elementos do sistema bancário.
Funções específicas do menu interagem com as classes para realizar operações bancárias básicas.
