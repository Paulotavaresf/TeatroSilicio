# Teatro do Silício

cadeira_1 = True
ca1 = 1
cadeira_2 = True
ca2 = 2
cadeira_3 = True
ca3 = 3
cadeira_4 = True
ca4 = 4
cadeira_5 = True
ca5 = 5

print("Seja Bem-Vindo, ao Teatro do Silício")
while True:
    print("<<<<<<<<<<<<>>>>>>>>>>>>")
    print("1- Reservar assento.")
    print("2- Cancelar Reserva.")
    print("3- Encerrar Atendimento.")
    print("<<<<<<<<<<<<>>>>>>>>>>>>")
    print()
    resp = int(input("Qual seu desejo? "))
    
    
    if resp == 1:
        if (cadeira_1 == False) and (cadeira_2==False) and (cadeira_3 == False) and (cadeira_4 == False) and (cadeira_5 == False):
            print("----------------------------------")
            print()
            print("TODOS OS ASSENTOS ESTÃO OCULPADOS!")
            print()
            print("----------------------------------")
            break
        else:
            print("A- ",ca1,ca2,ca3,ca4,ca5)
            print()
            print("     PALCO")
            print("     -----")
            assent = int(input("Qual assento deseja ocupar? "))
            print()
            
        if assent > 5:
            print("#################################")
            print("            ATENÇÃO")
            print("ESCOLHA UM ASSENTO DISPONÍVEL ENTRE 1 E 5")
            print("Por Favor, reserve outro assento!")
            print("#################################")
            print()
            print()
            
        if assent == 1:
                if cadeira_1 == False:
                    print("#################################")
                    print("            ATENÇÃO")
                    print("Assento reservado por : ",nome1)
                    print("Por Favor, reserve outro assento!")
                    print("#################################")
                    print()
                    print()
                else: 
                    cadeira_1 = False
                    ca1 = "X"
                    nome1 = str(input("Digite seu nome: "))
                    id1 = int(input("Digite seu ID: "))
                    print()
                    print("Reserva Concluída!")
                    print()
        elif  assent == 2:
                if cadeira_2 == False:
                    print("#################################")
                    print("            ATENÇÃO")
                    print("Assento reservado por : ",nome2)
                    print("Por Favor, reserve outro assento!")
                    print("#################################")
                    print()
                    print()
                else: 
                    cadeira_2 = False
                    ca2 = "X"
                    nome2 = str(input("Digite seu nome: "))
                    id2 = int(input("Digite seu ID: "))
                    print()
                    print("Reserva Concluída!")
                    print()
        elif  assent == 3:
                if cadeira_3 == False:
                    print("#################################")
                    print("            ATENÇÃO")
                    print("Assento reservado por : ",nome3)
                    print("Por Favor, reserve outro assento!")
                    print("#################################")
                    print()
                    print()
                else: 
                    cadeira_3 = False
                    ca3 = "X"
                    nome3 = str(input("Digite seu nome: "))
                    id3 = int(input("Digite seu ID: "))
                    print()
                    print("Reserva Concluída!")
                    print()
        elif  assent == 4:
                if cadeira_4 == False:
                    print("#################################")
                    print("            ATENÇÃO")
                    print("Assento reservado por : ",nome4)
                    print("Por Favor, reserve outro assento!")
                    print("#################################")
                    print()
                    print()
                else: 
                    cadeira_4 = False
                    ca4 = "X"
                    nome4 = str(input("Digite seu nome: "))
                    id4 = int(input("Digite seu ID: "))
                    print()
                    print("Reserva Concluída!")
                    print()
        elif  assent == 5:
                if cadeira_5 == False:
                    print("#################################")
                    print("            ATENÇÃO")
                    print("Assento reservado por : ",nome5)
                    print("Por Favor, reserve outro assento!")
                    print("#################################")
                    print()
                    print()
                else: 
                    cadeira_5 = False
                    Ca5 = "X"
                    nome5 = str(input("Digite seu nome: "))
                    id5 = int(input("Digite seu ID: "))
                    print()
                    print("Reserva Concluída!")
                    print()

    elif resp == 2:
        print("A- ",ca1,ca2,ca3,ca4,ca5)
        print()
        print("     PALCO")
        print("     -----")
        desistir = int(input("Qual seu assento? "))
        print()
        if desistir == 1 and cadeira_1 == True:
            print("Este assento não foi reservado!")
            break
        elif desistir == 1 and cadeira_1 == False:
            nome6 = nome1
            id6 = id1
        if desistir == 2 and cadeira_2 == True:
            print("Este assento não foi reservado!")
            break
        elif desistir == 2 and cadeira_2 == False:
            nome6 = nome2
            id6 = id2
        if desistir == 3 and cadeira_3 == True:
            print("Este assento não foi reservado!")
            break
        elif desistir == 3 and cadeira_3 == False:
            nome6 = nome3
            id6 = id3
        if desistir == 4 and cadeira_4 == True:
            print("Este assento não foi reservado!")
            break
        elif desistir == 4 and cadeira_4 == False:
            nome6 = nome4
            id6 = id4
        if desistir == 5 and cadeira_5 == True:
            print("Este assento não foi reservado!")
            break
        elif desistir == 5 and cadeira_5 == False:
            nome6 = nome5
            id6 = id5
        elif desistir > 5 and desistir <=0:
             print("Resposta Inválida!")
             break
        nome7 = str(input("Qual nome que está na reserva? "))
        id7 = int(input("Qual o ID que está na reserva? "))
        print()
        if nome7 == nome6 and id6 == id7:
            if desistir == 1:
                cadeira_1 = True
                ca1 = 1
                print("Reserva Cancelada!")
                print()
            elif desistir == 2:
                cadeira_2 = True
                ca2 = 2
                print("Reserva Cancelada!")
                print()
            elif desistir == 3:
                cadeira_3 = True
                ca3 = 3
                print("Reserva Cancelada!")
                print()
            elif desistir == 4:
                cadeira_4 = True
                ca4 = 4
                print("Reserva Cancelada!")
                print()
            elif desistir == 5:
                cadeira_5 = True
                ca5 = 5
                print("Reserva Cancelada!")
                print()
        else:
             print()
             print("Informações Inválidas!")
                
        

    elif resp == 3:
        print("Encerrando Atendimento...")
        break

    elif resp > 3 and resp <= 0:
        print("Digite uma opção válida! ")