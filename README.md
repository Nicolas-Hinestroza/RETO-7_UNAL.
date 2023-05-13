# RETO-9_UNAL.
Desarrolle la mayoría de ejercicios en clase. Para cada punto cree un programa individual. Al finalizar suba todo a un repo y subalo al canal reto_9 en slack.

- **1. De los retos anteriores seleciones 3 funciones y escribalas en forma de lambdas.**

- 1.1

![image](https://github.com/Nicolas-Hinestroza/RETO-9_UNAL../assets/124611099/8f4bba95-5ef1-4329-b053-8b0f4bb3ee1c)

    # 1.1 De los retos anteriores seleciones 3 funciones y escribalas en forma de lambdas.

    if __name__ == "__main__": # Llamamos la funcion principal
        N = int(input("Escriba la cantidad de gallinas: ")) # Primero vamos a definir N como la variable que el programa va a leer
        M = int(input("Escriba la cantidad de gallos: ")) # Primero vamos a definir M como la variable que el programa va a leer
        K = int(input("Escriba la cantidad de pollitos: ")) # Primero vamos a definir K como la variable que el programa va a leer
        peso_carne = lambda N, M, K : (N * 6) + (M * 7) + (K * 1) # Definimos la variable peso_carne con la funcion lambda con las variables N, M y K
        peso = peso_carne(N, M, K)# Definimos peso igual a peso_carne de las variables N, M y K
        print ("La cantidad de carne es " + str(peso) + "Kg") # Imprimimos  el resultado de la funcion lambda es decir imprimimos el peso total
        
- 1.2

![image](https://github.com/Nicolas-Hinestroza/RETO-9_UNAL../assets/124611099/79fec0b1-62f9-4503-9627-adeddabd3139)

    # 1.2 De los retos anteriores seleciones 3 funciones y escribalas en forma de lambdas.

    import math #Importamos la libreria que vamos a usar

    if __name__== "__main__": # Llamamos la funcion principal
        r1 = float(input("Escribe el valor del primer radio ")) # Primero vamos a definir r1 como la variable que el programa va a leer
        r2 = float(input("Escriba el valor del segundo radio ")) # Primero vamos a definir r2 como la variable que el programa va a leer
        h = float(input("Escriba el valor de la altura ")) # Primero vamos a definir h como la variable que el programa va a leer
        volumen_figura = lambda r1, r2, h : ((4/3) * math.pi * (r1)**3) + ((1/3) * h * math.pi * (r2)**2) # Definimos la variable volumen_figura con la funcion lambda con las variables r1, r2 y h
        area_figura = lambda r1, r2, h : (4 * math.pi * (r1)**2) + (math.pi * (h * r2) + math.pi * (r2)**2) # Definimos la variable area_figura con la funcion lambda con las variables r1, r2 y h
        volumen = volumen_figura (r1, r2, h) # Definimos volumen igual a volumen_figura de las variables r1, r2 y h
        area = area_figura (r1, r2, h) # Definimos area igual a area_figura de las variables r1, r2 y h
        print("El volumen de toda la figura es: " + str(volumen)) # Imprimimos  el resultado de la funcion lambda es decir imprimimos el volumen de la figura
        print("El area de toda la figura es: " + str(area)) # Imprimimos  el resultado de la funcion lambda es decir imprimimos el area de la figura

- 1.3

![image](https://github.com/Nicolas-Hinestroza/RETO-9_UNAL../assets/124611099/bfba732d-49eb-4dd7-a251-42fb42be4511)

    # 1.3 De los retos anteriores seleciones 3 funciones y escribalas en forma de lambdas.

    if __name__ == "__main__":  # Llamamos la funcion principal
       C = int(input("Escriba la cantidad de contagiados actuales: ")) # Primero vamos a definir C como la variable que el programa va a leer
       D = int(input("Escriba la cantidad de dias transcurridos: ")) # Primero vamos a definir D como la variable que el programa va a leer
       Contagiados = lambda C, D : C * (2**D) # Definimos contagiados como una funcion lambda nos devuelve a C multiplicado por 2 elevado a la D
       Co = Contagiados (C, D) # Definimos Co igual a Contagiados de las variables C y D
       print ("El numero de contagiados despues de", D, "dias es de " + str(Co)) # Imprimimos  el resultado de la funcion lambda

-  **2. De los retos anteriores seleciones 3 funciones y escribalas con argumentos no definidos (*args).**

- 2.1

![image](https://github.com/Nicolas-Hinestroza/RETO-9_UNAL../assets/124611099/a4f7b8ca-4593-450a-9259-218cabeda857)

    def factorial(*args): # Definimos la funcion factorial con args
        for y in args: # Para y en un rango de args
            print(y) # Imprimimos y
            return y # Nos develve el resultado de y
    def factorial2(y): # Definimos la funcion factorial2 con args  
        x = 1 # Definimos la variable x = 1
        for z in range(1,y+1): # Para z en un rango de 1 hasta y + 1
            x *= z # Definimos la variable z como x multiplicado a la z
            z -= 1 # Definimos z como z menos 1
        return x # Nos devuelve el resultado de x

    if __name__ == "__main__":  # Lamamos la Funcion principal
        n = int(input("Escribe un valor: ")) # Primero vamos a definir n como la variable que el programa va a leer
        print("El factorial del valor " + str(n) + " es: " + str(factorial2(n))) # cuando se complete el proceso se imprimira el numero digitado (n) y el factorial (f)
          
- 2.2

![image](https://github.com/Nicolas-Hinestroza/RETO-9_UNAL../assets/124611099/d0b6900e-3f53-4a27-a8fe-6e48c9420232)

     # 2.2 De los retos anteriores seleciones 3 funciones y escribalas con argumentos no definidos (*args).

    def Promedio(*args): # Definimos la funcion promedio con args
      z = 0 # Definimos la variable z = 0
      for n in args: # Para n en args
        z +=  n # Definimos a z como la suma de z 
      z = z // 5 # Definimos a z como la division de los valores que ya venian anteriormente y 5
      return z # Nos devuelve el resultado de z

    if __name__ == "__main__": # Llamamos la funcion principal 
      a = int(input("Ingrese numero a: ")) # Definimos a como la variable que recibimos
      b = int(input("Ingrese numero b: ")) # Definimos b como la variable que recibimos
      c = int(input("Ingrese numero c: ")) # Definimos c como la variable que recibimos
      d = int(input("Ingrese numero d: ")) # Definimos d como la variable que recibimos
      e = int(input("Ingrese numero e: ")) # Definimos e como la variable que recibimos
      print("Los numeros que escribiste son", a, b, c, d, e) #Imprimimos todas las variables
      print("El promedio de los numeros que escribiste es: " + str(Promedio(a, b, c, d, e))) # Imprimimos el resultado 
        
- 2.3

![image](https://github.com/Nicolas-Hinestroza/RETO-9_UNAL../assets/124611099/742c3a13-6bc1-4aea-a63e-48020bebcb21)

    # 2.3 De los retos anteriores seleciones 3 funciones y escribalas con argumentos no definidos (*args). 

    def potencia(*args): # Definimos la funcion potencia con args
        a = 1 # Definimos la variable a = 1
        for i in args: # Para i en args
            a = 2 ** i # a es igual a 2 elevado i
            return a # Nos devuelve el resultado de la potencia

    if __name__ == "__main__": # Llamamos la funcion principal 
        n = int(input("Escribe un valor: ")) # Definimos n como la variable que recibimos
        print("2 al elevarlo a la potencia " + str(n) + " es igual a: " + str(potencia(n))) # Imprimimos el resultado 

- **3. Escriba una función recursiva para calcular la operación de la potencia.** 

![image](https://github.com/Nicolas-Hinestroza/RETO-9_UNAL../assets/124611099/6ef4dfe7-d7d4-419f-8258-49ebc9daae7d)

    # 3. scriba una función recursiva para calcular la operación de la potencia.

    def potenciarecursivo(a, b): # Definimos la funcion potenciarecursivo para las variables a y b 
        if b == 0: # Si b == 0 entonces
            return 1 # Nos devuelve 1 ya que todo numero elevado 0 da 1
        elif a == 0: # Si a == 0 entonces
            return 0 # Nos devuelve 0 ya que 0 elevado a cualquier numero da 0
        if b == 1: # Si b == 1 entonces
            return a # Nos devuelve 1 ya que cualquier numero elevado 1 es igual al numero 
        else: # Si no se cumple cualquiera de las anteriores entonces
            return a * potenciarecursivo(a, b-1) # Nos devuelve a elevado al pontenciarecursivo de a y b - 1
    
    if __name__ == "__main__": # Llamamos la funcion principal  
        a = int(input("Escribe un valor real : ")) # Definimos a a como la variable que recibimos
        b = int(input("Escribe un valor real para que sea una potencia: ")) # Definimos a b como la variable que recibimos
        print(str(a) + " al elevarlo por " + str(b) + " es igual a: " + str(potenciarecursivo(a, b))) # Imprimimos el resultado  

- **4. Realice pruebas para calcular fibonacci con iteración o con recursión. Determine desde que número de la serie la diferencia de tiempo se vuelve significativa.**

![image](https://github.com/Nicolas-Hinestroza/RETO-9_UNAL../assets/124611099/e4ae9ea4-8298-4344-a2b9-7255f347d3b4)

    # 4. Realice pruebas para calcular fibonacci con iteración o con recursión. Determine desde que número de la serie la diferencia de tiempo se vuelve significativa. 

    import time  #Importamos la libreria que vamos a usar

    def Fibo(n): # Definimos la funcion fibo con la variable n
      i = 1 # Definimos la variable 1 = 1 
      a = 0 # Definimos la variable a = 0 
      b = 1 # Definimos la variable b = 1 
      while(i <= n): # mientras que i sea menor o igual que n haga
        sumFibo = a + b # DEfinimos la variable sumFibo que seria el resultado de a + b
        a = b # a quedaria valiendo b
        b = sumFibo # y b quedaria valiendo sumFibo
        i += 1 # le sumamos uno a i para que la serie de fibo se calcule hasta n
      return sumFibo # Nos devuelve el resultado de sumFibo

    if __name__ == "__main__":  # Llamamos la Función principal
      n = int(input("Escribe un valor: ")) # Definimos n como la variable que recibimos
      start_time1 = time.time() # Utilizamos las formulas brindadas para calcular el tiempo de la serie
      end_time1 = time.time() # Utilizamos las formulas brindadas para calcular el tiempo de la serie
      timer1 = end_time1 - start_time1 # Definimos la varable timer 1
      print("La serie de Fibonacci hasta el numero " + str(n) + " es " + str(Fibo(n))) # Imprimimos el resultado de la serie de fibo
      print("Fibonacci calculado de forma iterativa tardo: ", timer1) # Imprimimos el tiempo que tarda en calcular la serie

- **5. Crear cuenta en stackoverflow y adjuntar imagen en el repo.**

![image](https://user-images.githubusercontent.com/124611099/236643870-49ea32ef-3c5a-43e1-b804-a5bb18108af1.png)

- **5. Ir a linkedin y crear perfil.**

![image](https://user-images.githubusercontent.com/124611099/236644018-65cf6ffe-1341-4c63-94b6-7349e3596d8f.png)

Link: linkedin.com/in/nicolas-david-hinestroza-hernandez-90586b275

