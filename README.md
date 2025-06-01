1. Imprime un listado con los números del 1 al 100 cada uno con su respectivo cuadrado.

       print("Numero-Cuadrado")
       for i in range(1, 101):
         print(f"{i}\t{i**2}")

2. Imprimir un listado con los números impares desde 1 hasta 999 y seguidamente otro listado con los números pares desde 2 hasta 1000.

       print("Numeros impares del 1 al 999:")
       for i in range(1, 1000, 2):
           print(i, end=' ')
       print("//")
       print("Numeros pares del 2 al 1000:")
       for i in range(2, 1001, 2):
           print(i, end=' ')
   
3. Imprime los números pares en forma descendente hasta 2 que son menores o iguales a un número natural n ≥ 2 dado.
    
       numero = int(input("Ingrese un número natural mayor que 2: "))
       while numero>=2:
             #Determiar si n es par
            if  numero % 2 == 0:
               print(numero)
               numero=numero-1

4. Imprimir el factorial de un número natural n dado.
    
       n = int(input("Ingrese un numero natural para calcular su factorial: "))
       if n < 0:
            print("El factorial no esta definido para numeros negativos.")
       factorial = 1
       for i in range(1, n + 1):
            factorial *= i
       print(f"El factorial de {n} es: {factorial}")

5. Implementar un programa que ingrese un número de 2 a 50 y muestre sus divisores.

       # Agregar un numero entre 1 y 50
       # Otener los divisores de ese numero
           numero = int(input("Ingrese un número entre 2 y 50: "))
       #Inicializacion

           mitad: int=numero//2+1
       #Condicion

           while mitad >=2:
       #Instrucciones del ciclo
       #Nesesito verificar si mitad es divisor de n

               if numero % mitad == 0:
                  print ("El nuumero "+ str(mitad)+ " Es divisor")
               mitad = mitad -1
       #Actualizacion

6. Implementar el algoritmo que muestre los números primos del 1 al 100. Nota: use funciones
   
          def es_primo(n):
           if n < 2:
        return False
           for i in range(2, int(n**0.5) + 1):
               if n % i == 0:
                   return False
           return True

       print("Números primos del 1 al 100:")
       for i in range(1, 101):
           if es_primo(i):
               print(i, end=' ')
