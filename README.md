user="WEYMAR"
password="weymar"
while True:
    usuario=input("INTTRODUSCA USUARIO: ")
    contra=input("INTRODUSCA CONTRASENA: ")
    al = ["a", "b", "c", "d", "e", "f", "g", "h", "i", "j", "k", "l", "m", "n", "o", "p", "q", "r", "s", "t", "u", "v",
          "w", "x", "y", "z"]
    num = [0, 1, 1, 2, 3, 5, 8, 13, 21, 34, 55, 89, 144, 233, 377, 610, 987, 1597, 2584, 4181, 6765, 10946, 17711,
           28657, 46368, 75025]
    contra = contra.lower()
    v = ""
    for i in range(len(contra) + 1):
        y = contra[i - 1:i]
        for j in range(len(al)):
            if y == al[j]:
                NUM = str(num[j])
                v = v + NUM

    if usuario==user and contra==password:
        print("\n")
        print("LA CONTRASENA INCRIPTADA ES: ", v)
        print(("\n"))
        print("BIENVENIDO AL SISTEMA WEYMAR VILLCA (UMSA) LAB111 ")
        print("***********************")
        print("  ELIJA ALGUNA OBSION: ")
        print("***********************")
        print(" 1. PRIMERA OPERACION: ")
        print(" 2. SEGUNDA OPERACION: ")
        print(" 3. TERCERA OPERACION: ")
        print(" 4. CUARTA OPERACION:  ")
        print(" 5. SALIR:             ")
        print("***********************")
        opcion=int(input("DIGITE OBSION: "))
        print("HA SELECCIONADO LA OPCION: ",opcion)
        if opcion==1:
            print("*************************")
            print("DIVISION DE DOS NUMEROS: ")
            print("*************************")
            a=int(input("INTRO A: "))
            b=int(input("INTRO B: "))
            c=a/b
            v=a%b
            print(c)
            print(v)
            print("***********************")
            print("  ELIJA ALGUNA OBSION: ")
            print("***********************")
            print(" 1. PRIMERA OPERACION: ")
            print(" 2. SEGUNDA OPERACION: ")
            print(" 3. TERCERA OPERACION: ")
            print(" 4. CUARTA OPERACION:  ")
            print(" 5. SALIR:             ")
            print("***********************")
            opcion=int(input("LA OPERACION A TERMINADO VUELVA A SELECCIONAR OBSION: "))
            print("HA SELECCIONADO LA OBSION ",opcion)
        if opcion==2:
            print("***********")
            print("DIVISORES: ")
            print("***********")
            aux=999999
            while True:
                n=int(input("intro n"))
                if n>aux:
                    break
            aux=1
            cont=1
            while aux<n:
                c=n%cont
                if c==0:
                    print(cont,end=",")

                cont=cont+1

            aux=aux+1



        if opcion==3:
            print("******************")
            print("NUMEROS CAPICUAS: ")
            print("******************")
            aux=9
            while True:
                n=int(input("intro n"))
                if n>aux:
                    break
            centena=n/100
            decena=(n%100)/10
            unidad=(n%100)%10
            if (centena==unidad):
                print("el numero NO es capicua: ")
            else:
                print("el numero es capicua: ")
        print("***********************")
        print("  ELIJA ALGUNA OBSION: ")
        print("***********************")
        print(" 1. PRIMERA OPERACION: ")
        print(" 2. SEGUNDA OPERACION: ")
        print(" 3. TERCERA OPERACION: ")
        print(" 4. CUARTA OPERACION:  ")
        print(" 5. SALIR:             ")
        print("***********************")
        opcion = int(input("LA OPERACION A TERMINADO VUELVA A SELECCIONAR OBSION: "))
        print("HA SELECCIONADO LA OBSION ", opcion)

        if opcion==4:
            print("****************")
            print("CAMBIO DE BASE: ")
            print("****************")
            n=int(input("introdusca n: "))
            b=int(input("introdusca b: "))
        print("***********************")
        print("  ELIJA ALGUNA OBSION: ")
        print("***********************")
        print(" 1. PRIMERA OPERACION: ")
        print(" 2. SEGUNDA OPERACION: ")
        print(" 3. TERCERA OPERACION: ")
        print(" 4. CUARTA OPERACION:  ")
        print(" 5. SALIR:             ")
        print("***********************")
        opcion = int(input("LA OPERACION A TERMINADO VUELVA A SELECCIONAR OBSION: "))
        print("HA SELECCIONADO LA OBSION ", opcion)
        if opcion==5:
            print("***************************************************")
            print("NO ESTA DEL TODO COMPLETO PERO ISE LO QUE PUDE     ")
            print("ESPERO QUE NO ME REPRUEBE ARUN TE AMO XD NO ME REP.")
            print("***************************************************")
        break
    else:
        print("SIGUE PARTISIPANDO BRO CONTRASENA INCORRECTA")
