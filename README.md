# DESAFIO-DIO-CONTA-BANCARIA-2
CONTA BANCARIA 2 - SEGUNDO DESAFIO PYTHON


________________________________________
💻 Sistema Bancário em Python
Este projeto é um sistema bancário simples feito em Python, que simula operações de depósito, saque, criação de usuários e contas, exibição de extrato e listagem de contas.

🧠 Funcionalidades
•	Criar usuários
•	Criar contas bancárias
•	Realizar depósitos
•	Realizar saques com limite
•	Exibir extrato de movimentações
•	Listar todas as contas criadas
•	Menu interativo para o usuário
________________________________________

🧩 Explicação do Código
1. menu()
Exibe um menu interativo com as opções disponíveis para o usuário. Utiliza a biblioteca textwrap para formatar o texto com indentação correta.
________________________________________

2. depositar(saldo, valor, extrato, /)
Recebe os dados por posição:
•	Se o valor for positivo, ele é somado ao saldo e registrado no extrato.
•	Se o valor for inválido, mostra uma mensagem de erro.
Retorna o novo saldo e o extrato atualizado.
________________________________________

3. sacar(*, saldo, valor, extrato, limite, numero_saques, limite_saques)
Recebe os dados por nome:
•	Verifica se o valor excede o saldo, o limite por saque ou o número máximo de saques.
•	Se tudo estiver certo, realiza o saque e atualiza o extrato e a contagem de saques.
Retorna o novo saldo e o extrato.
________________________________________

4. exibir_extrato(saldo, /, *, extrato)
Mostra o extrato completo com todas as movimentações e o saldo atual. Se não houver movimentações, informa isso ao usuário.
________________________________________

5. criar_usuario(usuarios)
Cria um novo usuário bancário:
•	Pede CPF, nome, data de nascimento e endereço.
•	Verifica se o CPF já existe usando a função filtrar_usuario.
•	Adiciona o usuário à lista usuarios.
________________________________________

6. filtrar_usuario(cpf, usuarios)
Procura um usuário pelo CPF.
•	Se encontrar, retorna o usuário.
•	Caso contrário, retorna None.
________________________________________

7. criar_conta(agencia, numero_conta, usuarios)
Cria uma nova conta bancária:
•	Solicita o CPF do usuário.
•	Se o usuário existir, cria uma conta com número e agência.
•	Retorna a nova conta para ser armazenada.
________________________________________

8. listar_contas(contas)
Percorre a lista de contas e exibe os dados de cada conta formatados com a agência, número da conta e nome do titular.
________________________________________

9. main()
Função principal que:
•	Define variáveis globais como saldo, limite, extrato, usuários e contas.
•	Executa o loop principal do sistema, lendo a opção escolhida no menu.
•	Chama a função correspondente para cada opção.
________________________________________

🚀 Como usar
1.	Execute o arquivo .py com Python 3 instalado.
2.	Use as opções do menu para interagir com o sistema.
________________________________________

📌 Observações
•	Cada saque tem um limite de R$ 500,00.
•	O limite de saques por sessão é 3.
•	O extrato registra todas as movimentações de forma detalhada.
•	O CPF é usado para identificar exclusivamente cada usuário.
________________________________________

