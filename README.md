# RETO-7_UNAL.
Desarrolle la mayoría de ejercicios en clase. Para cada punto cree un programa individual. Al finalizar suba todo a un repo y subalo al canal reto_9 en slack.

- **1. De los retos anteriores seleciones 3 funciones y escribalas en forma de lambdas.**

- 1.1



      # 1.1 De los retos anteriores seleciones 3 funciones y escribalas en forma de lambdas.

      if __name__ == "__main__":  #Funcion principal
          N = int(input("Escriba la cantidad de gallinas: "))
          M = int(input("Escriba la cantidad de gallos: "))
          K = int(input("Escriba la cantidad de pollitos: "))
          peso_carne = lambda N, M, K : (N * 6) + (M * 7) + (K * 1)
          peso = peso_carne(N, M, K)
          print ("La cantidad de carne es " + str(peso) + "Kg")
- 1.2



      # 1.2 De los retos anteriores seleciones 3 funciones y escribalas en forma de lambdas.
      import math
      if __name__== "__main__":
          r1 = float(input("Escribe el valor del primer radio "))
          r2 = float(input("Escriba el valor del segundo radio "))
          h = float(input("Escriba el valor de la altura "))
          volumen_figura = lambda r1, r2, h : ((4/3) * math.pi * (r1)**3) + ((1/3) * h * math.pi * (r2)**2)
          area_circulo = lambda r1, r2, h : (4 * math.pi * (r1)**2) + (math.pi * (h * r2) + math.pi * (r2)**2)
          volumen = volumen_figura (r1, r2, h)
          area = area_circulo (r1, r2, h)
          print("el volumen de toda la figura es: " + str(volumen))
          print("el area de toda la figura es: " + str(area))
- 1.3



      # 1.3 De los retos anteriores seleciones 3 funciones y escribalas en forma de lambdas.
      if __name__ == "__main__":  #Funcion principal
         C = int(input("Escriba la cantidad de contagiados actuales: "))
         D = int(input("Escriba la cantidad de dias transcurridos: "))
         Contagiados = lambda C, D : C * (2**D)
         Co = Contagiados (C, D)
         print ("El numero de contagiados despues de", D, "dias es de " + str(Co))


-  **2. De los retos anteriores seleciones 3 funciones y escribalas con argumentos no definidos (*args).**

- 2.1



      # 2.1 De los retos anteriores seleciones 3 funciones y escribalas con argumentos no definidos (*args).
      def factorial(*args):
          for y in args:
              print(y)
              return y
      def factorial2(y):    
          x = 1
          for z in range(1,y+1):
              x *= z
              z -= 1
          return x

      if __name__ == "__main__":  #Funcion principal
          n = int(input("Escribe un valor: ")) # Primero vamos a definir n como la variable que el programa va a leer
          print("El factorial del valor " + str(n) + " es: " + str(factorial2(n))) # cuando se complete el proceso se imprimira el numero digitado (n) y el factorial (f)
          
- 2.2

      # 2.2 De los retos anteriores seleciones 3 funciones y escribalas con argumentos no definidos (*args).
      def Promedio(*args):
        z = 0
        for n in args:
          z +=  n
        z = z // 5 
        return z

      if __name__ == "__main__":
        a = int(input("Ingrese numero a: "))
        b = int(input("Ingrese numero b: "))
        c = int(input("Ingrese numero c: "))
        d = int(input("Ingrese numero d: "))
        e = int(input("Ingrese numero e: "))
        print("El promedio de los numeros que escribiste es: " + str(Promedio(a, b, c, d, e)))
        
- 2.3

      # 2.3 De los retos anteriores seleciones 3 funciones y escribalas con argumentos no definidos (*args). 
      def potencia(*args):
          a = 1
          for i in args:
              a = 2 ** i
              return a

      if __name__ == "__main__":
          n = int(input("Escribe un valor: "))
          print("2 al elevarlo a la potencia " + str(n) + " es igual a: " + str(potencia(n)))

- **3. Escriba una función recursiva para calcular la operación de la potencia.** 

      # 3. scriba una función recursiva para calcular la operación de la potencia.
      def potenciarecursivo(a, b):
          if b == 0:
              return 1
          elif a == 0:
              return 0
          if b == 1:
              return a
          else:
              return a * potenciarecursivo(a, b-1)
    
      if __name__ == "__main__":    
          a = int(input("Escribe un valor real : "))
          b = int(input("Escribe un valor real para que sea una potencia: "))
          print(str(a) + " al elevarlo por " + str(b) + " es igual a: " + str(potenciarecursivo(a, b)))

- **4. Realice pruebas para calcular fibonacci con iteración o con recursión. Determine desde que número de la serie la diferencia de tiempo se vuelve significativa.**



- **5. Crear cuenta en stackoverflow y adjuntar imagen en el repo.**

![image](https://user-images.githubusercontent.com/124611099/236643870-49ea32ef-3c5a-43e1-b804-a5bb18108af1.png)

- **5. Ir a linkedin y crear perfil.**

![image](https://user-images.githubusercontent.com/124611099/236644018-65cf6ffe-1341-4c63-94b6-7349e3596d8f.png)

Link: linkedin.com/in/nicolas-david-hinestroza-hernandez-90586b275

