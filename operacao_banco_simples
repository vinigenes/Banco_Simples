menu = ' Bem vindo ao nosso Banco Simples, qual operação deseja realizar? \n [1] Depositar\n [2] Sacar\n [3] Extrato\n [4] Sair\n Digite a opção desejada: ' 

#O sistema deve permitir realizar 3 saque com limete máximo de R$ 500,00 por saque.
LIMITE_SAQUE = 3
limite = 500
extrato = ''
valor = 0
saldo = 0
numero_de_saques = 0

while True:
    menu_de_operacao = input (menu)
    
    if menu_de_operacao == '1':
        valor = float(input("Informe o valor do depósito: "))
        
        if valor > 0:
            saldo += valor
            extrato += f"Depósito: R$ {valor:.2f}" 
            print(saldo)
        else: 
            print("Operação falhou, o valor não é valido.")
            
    elif menu_de_operacao == '2':
        valor = float(input("Informe o valor do saque: "))
        
        excedeu_saldo = valor > saldo
        
        excedeu_limite = valor > limite 
        
        excedeu_saques = numero_de_saques  >= LIMITE_SAQUE
            
        if excedeu_saldo:
                print ("Operação falhou! Você não tem saldo suficiente.")
        elif excedeu_limite:
                print ("Operação falhou! Você excedeu o limite de saque por operação")
        elif excedeu_saques:
                print ("Operação falhou! Você número excedeu o número de saques.") 
        elif valor > 0:
            saldo -= valor
            extrato += f"Saque: R$ {valor:.2f}\n"
            numero_de_saques +=1
            
        else :
            print("Operação falhou! O valor informado é inválido")
    
    elif menu_de_operacao == '3':
        print("\n================ EXTRATO ================")
        print("Não foram realizadas movimentações." if not extrato else extrato)
        print(f"\nSaldo: R$ {saldo:.2f}")
        print("==========================================")
    
    elif menu_de_operacao == '4':
        print('Obrigado pela utilização do nosso banco!')
        break
    else:
        print("Operação inválida, por favor selecione novamente a operação desejada.")
                
    
            
            

        
        
    



