![image](https://user-images.githubusercontent.com/52517310/60692597-60585800-9e9c-11e9-9c54-f42ede98dff3.png)


# programacionBasica
Ejercicios curso de programación básica TESH
#Python Programación basica TESH 
----
## 1.-Conceptos basicos y algoritmos
#### ¿Qué es python?

###### Es un lenguaje de programacion creado por Guido van Rossum a principio de los años 90´s,cuyo nombre esta inspirado en el grupo de comicos ingleses''monty python'',es un lenguaje similar a ''C'' ,pero con una sintaxis muy limpia y que favorece un codigo legible.
###### Lenguaje interpretado o escrito:Interpretado o de script es aquel que se ejecuta utilizando un programa intermediario que se llama *interprete*  en lugar de compilar el codigo al lenguaje maquina.
###### Todos nuestro programas deben guardarse con la extension.py, para Correrlos utilizaremos Anaconda Prompt/spyder.


## Conceptos:

###### Los tipos de datos basicos se dividen en numeros,como pueden ser:

###### variable:Una variable es donde se guarda (y se recupera) datos que se utilizan en un programa.

###### Cadena de texto: Se representa con un *string*

###### Numero entero: integer=int
###### Numero decimal: float

###### Concatenar : Unir variables del tipo string en una sola.

###### Ejemplo cadenas de texto que pida al usuario ingresar su nombre para despues imprimirlo:
    nombre=input('Ingresa tu nombre:')
    print('hola',nombre)



----
## Operadores
###### Los numeros complejos son aquellos que tienen una parte imaginaria, para definir una variable compleja utilizamos el termino: *complex*
###### Operadores:
* suma= +
* resta= -
* multiplicacion= *
* exponente= **
* division= /
* division entera= //
* modulo=%

###### Ejemplo: escriba un programa que lea 2 numeros enteros y los guarde en las variables a y b y efectue las operaciones del apartado *operadores*

    a=int(input('Ingrese un numero entero'))
    b=int(input('Ingrese un segundo numero entero'))
    import math
    suma=a+b
    resta=b-a
    multi=a*b
    modulo=a%b
    division=a/b
    exponente= a**b

    print('la suma es:',suma,)
    print('la resta es:',resta,)
    print('el producto es:',multi,)
    print('El cociente es:',modulo,)
    print('El residuo es:',division,)
    print('El resultado de elevar a por 
    b:',exponente,)
    print('el logaritmo de 10 de a es:',math.log(a))

###### Ejemplo: La eficiencia de la gasolina en los vehículos esta expresada en millas por galón,En mexico esta expresada en litros por cada 100km/L, determinar como convertir de MPG A L/100KM,escriba un programa que lea un valor en unidades americanas y las convierta a unidades mexicanas.

    milla=float(input('ingresa el numero de MPG:'))
    conversion=235.215/milla 
    print('la conversion a unidades mexicanas 
    es:',conversion,'L/100km')

###### Realiza un programa que calcule el area de un campo de futbol y que muestre el resultado en metros,pies y acres.

    largo=float(input('cuanto mide el largo del campo 
    de futbol: '))
    ancho=float(input('cuanto mide el ancho del campo 
    de futbol: '))
    area=largo * ancho
    area2=area * 90.70
    area3=area2 / 43560
    print('el area del campo de futbol es' ,area, 
    'metros cuadrados')
    print('el area del campo de futbol es' ,area2, 
    'en pies cuadrados')
    print('el area del campo de futbol es' , area3, 
    'en acres')




###### Ejemplo:Escriba un programa que calcule el area y volumen del circulo.
    import math
    radio=float(input('ingresa el radio;'))
    area= math.pi*(radio**2)
    volumen= 4/3*3.1416*(radio**3)

    print('el area del circulo es:',area,'cm 
    cuadrados')
    print('el volumen del circulo es:' ,volumen,'cm 
    cubicos')
###### Ejemplo:Escriba un programa que calcule los intereses generados a un plazo de 1 ,2 y 3 años. 

    inversion= float(input('Ingrese el monto que 
    desea invertir, Enter the amount:'))
    interes= inversion * 4 / 100
    a2= inversion * 2
    a3= inversion * 3
    print('El interes generado en su cuenta de ahorro 
    al cabo de 1 anio  es:',interes,'pesos')
    print('El interes generado en su cuenta de ahorro 
    al cabo de 2 anios es:',a2,'pesos') 
    print('El interes generado en su cuenta de ahorro 
    al cabo de 3 anios es:',a3,'pesos')

###### Escriba un programa que calcule los dias, minutos,segundos.

    dias=float(input('inserta el numero de dias: '))
    d=dias
    horas=float(input('inserta el numero de horas: 
    '))
    h=horas
    minutos=float(input('inserta el numero de 
    minutos: '))
    m=minutos
    segundos=float(input('inserta el numero de 
    segundos: '))
    s=segundos
    resultado=d * 86400
    resultado2= h * 3600
    resultado3= m * 60
    resultado4= s * 1
    resultado5= resultado + resultado2 + resultado3 + 
    resultado4
    print('en dias tienes' ,resultado,'segundos')
    print('en horas tienes' ,resultado2, 'segundos')
    print('en minutos tienes' ,resultado3,'segundos')
    print('en segundos tienes' 
    ,resultado4,'segundos')
    print('tienes un total de' 
    ,resultado5,'segundos')

###### Escriba un programa que mueste la hora actual.

    import time
    print('la hora actual es 
    ',time.strftime("%I:%M:%S"))
    print('la fecha actual es 
    ',time.strftime("%d/%m/%y"))

###### Escriba un programa que calcule el area de un triangulo utilizando la base y la altura.


    longitud=float(input('inserta cuando medira b: 
    '))
    b=longitud
    altura=float(input('inserta cuanto medira h: '))
    h=altura
    area= b * h / 2
    print('el area del triangulo es' ,area, 
    'centimetros cuadrados')


###### Ejemplo: Escriba un programa que lea un número entero positivo, n, del usuario y luego muestre el suma de todos los enteros de 1 a n. La suma de los primeros n enteros positivos puede ser calculado utilizando la fórmula:

    numero = int(input('ingresa un numero:'))
    suma= (numero * (numero+1))/2
    print(suma) 

###### Un minorista en línea vende dos productos: widgets y artilugios. Cada widget pesa 75 gramos Cada gizmo pesa 112 gramos. Escribe un programa que lea el número de widgets y el número de artilugios en un pedido del usuario. Entonces tu programa Debe calcular y mostrar el peso total del pedido.

    widgets=int(input('Ingresa el numero de widgets, 
    Enter your number of widgets:'))
    gizmo= int(input('Ingresa el numero de gizmos , 
    Enter your number of gizmos:'))
    peso1= widgets * 75
    peso2= gizmo * 112
    peso3= peso1 + peso2
    print('El peso de widgets es:',peso1,)
    print('El peso de gizmos es:',peso2,)
    print('El peso total es',peso3,'gramos')

###### Ejemplo:Realiza un programa que calcule el area de tu habitacion.

    largo= float(input('ingresa el largo de de tu 
    habitacion:'))
    ancho= float(input('ingresa el ancho de de tu 
    habitacion:'))
    area= largo * ancho
    print('el area de tu habitacion es',area,'metros 
    cuadrados')

###### Escriba un programa que calcule si el numero es PAR o IMPAR.

    n = int(input('Inserta cualquier numero: '))
    if n%2 == 0:
    print('El numero es par')
    elif n%2 != 0:
    print('El numero es inpar')



###### Escriba un programa que haga la conversion de pies y pulgadas a metros.


    pies= float(input("inserta elnumero de millas: 
    "))
    pulgadas= float(input("inserta el numero de 
    pulgadas: "))
    metros= 0.3048 * pies + 0.0254 * pulgadas
    print('tienes un equivalente de' ,metros, 
    'metros')

###### Ejemplo:La superficie de la Tierra es curva, y la distancia entre grados de longitud Varía con la latitud. Como resultado, encontrando la distancia entre dos puntos en la superficie La Tierra es más complicada que simplemente usar el teorema de Pitágoras. Sean (t1, g1) y (t2, g2) la latitud y longitud de dos puntos en la Tierra superficie. La distancia entre estos puntos, siguiendo la superficie de la Tierra, en kilómetros es: distancia = 6371.01 × arccos (sin (t1) × sin (t2) + cos (t1) × cos (t2) × cos (g1 - g2)) El valor 6371.01 en la ecuación anterior no se seleccionó al azar. Es El radio medio de la tierra en kilómetros. Cree un programa que permita al usuario ingresar la latitud y longitud de dos Puntos en la tierra en grados. Su programa debe mostrar la distancia entre Los puntos, siguiendo la superficie de la tierra, en kilómetros.

    from math import degrees,sin,cos,acos
    latitud=(float(input('ingresa latitud:')))
    longitud=(float(input('ingresa longitud:')))
    latitud2=(float(input('ingresa latitud:')))
    longitud2=(float(input('ingresa longitud:')))
    distancia= 
    6371.01*acos(sin(latitud)*sin(latitud2)
    +cos(latitud)*cos(latitud2)*cos(longitud- 
    longitud2))
    distancia2=degrees(distancia)
    print('la distancia es',distancia2,'km')

###### Escriba un programa que comienza leyendo la temperatura del usuario en grados Celsius. Entonces su programa debería mostrar la temperatura equivalente en grados Fahrenheit y grados Kelvin. Los cálculos necesarios para convertir entre diferentes Las unidades de temperatura se pueden encontrar en internet.
    
    celsius=input('ingrese la temperatura en grados 
    Celsius')
    kelvin= (celsius × 9/5)+32
    fa= celsius + 273.15
    print('la temp en grados kelvin es',kelvin)
    print('la temp en grados farenheit es',fa)


## 2.Control de flujo
###### Sistemas condicionales:Si un programa no fuera mas que una lista de ordenes a ejecutar de forma secuencial, uno por uno, no tendría mucha utilidad.

## Condicional if
###### La forma mas simple de una sentencia condicional es el if (del ingles''si'') seguido de la condicion a evaluar (:) y en la siguiente linea el indentado del 

condigo a ejecutar en caso que se cumpla dicha condición.
###### *comparaciones:*
* a==b   (a es igual a b)

* a!=b   (a no es igual a b)

* a < b  (a es menor que  b)
 
* a > b  (a es mayor que  b)

* a <= b (a es menor o igual que b)

* a >= b (a es mayor o igual que b)


###### elif nos servira para hacer una segunda comparacion, mientras que Else  se ocupara en caso de que las comparaciones no sean ciertas.

###### Ejemplo: Realiza la comparacion entre dos numeros enteros :
    a =input('ingrese un numero entero')
    b =input('ingrese un segundo numero entero')
    if b > a:
    print("b es mayor que a")
    elif a == b:
    print("a y b son iguales")
    else:
    print("a es mayor que b")

###### Escriba un programa que calcule el volumen de una esfera conociendo su radio.

    import math
    from math import pi
    radio=float(input('ingresa el radio de la esfera: 
    '))
    rad=radio
    resultado = 3.1416*(rad) **2 
    volumen = 4 / 3 * 3.1416 * (rad) ** 3
    print('tu area es' ,resultado,'centimetros 
    cuadrados' )
    print('el volumen de la esfera es' ,volumen, 
    'centimetros cubicos')

###### Realiza un programa que calcule los precios para botellas de diferente capacidad, las de 1 litro con un precio de $1 y las de 2 litros $2.50

    botella1=int(input('cuantas botellas de 1 litro o 
    menos traes: '))
    botella2=float(input('cuantas botellas de 1 litro 
    o mas traes: '))
    total=botella1 + botella2
    print('tienes un total de' ,total, 'botellas')
    precio1=botella1 * 1
    print('el precio de botellas de menos de 1 litro 
    es ',precio1,'pesos')
    precio2=botella2 * 2.50
    print('el precio de botellas de mas de 1 litro es 
    ',precio2,'pesos')
    precio= precio1 + precio2
    print('el precio total es' ,precio,'pesos')


----
###### Ejemplo:Se dice comúnmente que un año humano es equivalente a 7 años caninos. Sin embargo esto la simple conversión no reconoce que los perros alcanzan la edad adulta en aproximadamente dos años. Como resultado, algunas personas creen que es mejor contar cada uno de los dos primeros los años humanos como 10.5 años del perro, y luego cuentan cada año humano adicional como 4 perros años. Escribe un programa que implemente la conversión de años humanos a años de perros.descrito en el párrafo anterior. Asegúrese de que su programa funciona correctamente para conversiones de menos de dos años humanos y para conversiones de dos o más humanos años. Su programa debería mostrar un mensaje de error apropiado si el usuario ingresa un número negativo.

    humano = int(input("Ingresa la edad del perro en 
    anios humanos: "))

    if humano < 0:
	print("ingresa un numero positivo.")
	exit()
    elif humano <= 2:
	perro = humano * 10.5
    else:
	perro = 21 + (humano - 2)*4

    print("la edad en años perros es:", perro)

###### El zodiaco chino asigna animales a años en un ciclo de 12 años. Un ciclo de 12 años es Se muestra en la tabla de abajo. El patrón se repite desde allí, siendo 2012 otro. año del dragón, y 1999 siendo otro año de la liebre. Escriba un programa que lea un año del usuario y muestre el animal asociado con ese año. Su programa debería funcionar correctamente para cualquier año mayor o igual a cero, no solo a los que figuran en la tabla.

    year = int(input ("Ingrese su año de 
    nacimiento:"))
    if (año - 2000)% 12 == 0:
        signo = 'Dragón'
    elif (año - 2000)% 12 == 1:
        signo = 'Serpiente'
    elif (año - 2000)% 12 == 2:
         signo = 'Caballo'
    elif (año - 2000)% 12 == 3:
         signo = 'oveja'
    elif (año - 2000)% 12 == 4:
        signo = 'Mono'
    elif (año - 2000)% 12 == 5:
        signo = 'gallo'
    elif (año - 2000)% 12 == 6:
        signo = 'Perro'
    elif (año - 2000)% 12 == 7:
        signo = 'cerdo'
    elif (año - 2000)% 12 == 8:
        signo = 'Rata'
    elif (año - 2000)% 12 == 9:
         signo = 'buey'
    elif (año - 2000)% 12 == 10:
        signo = 'tigre'
         más:
    signo = 'liebre'

    print("Su signo del zodiaco:", signo)


###### Los horóscopos reportados comúnmente en los periódicos utilizan la posición del sol en el tiempo de nacimiento para tratar de predecir el futuro. Este sistema de astrología divide el año en doce signos del zodiaco.Escriba un programa que le pida al usuario que ingrese su mes y día de nacimiento. Entonces su programa debe informar el signo zodiacal del usuario como parte de una salida apropiada mensaje.

    day = int(input("ingresa el dia en que naciste "))
    
    month = input("ingresa el mes en que naciste ")
    if mes == 'diciembre':astro_sign = 'Sagitario' 
    if (day < 22) else 'capricorn'
    elif mes == 'enero': astro_sign = 'Capricornio' 
    if (day < 20) else 'aquarius'
    elif mes == 'febrero':astro_sign = 'Acuario' if 
    (day < 19) else 'pisces'
    elif mes == 'marzo':
    astro_sign = 'Piscis' if (day < 21) else 'aries'
    elif mes == 'abril': astro_sign = 'Aries' if (day 
    < 20) else 'taurus'
    elif mes == 'mayo':
    astro_sign = 'Taurus' if (day < 21) else 'gemini'
    elif mes == 'junio':
    astro_sign = 'Geminis' if (day < 21) else ' 
    cancer'
    elif mes == 'julio': astro_sign = 'Cancer' if 
    (day < 23) else 'leo'
    elif mes == 'augosto':
    astro_sign = 'Leo' if (day < 23) else 'virgo'
    elif mes == 'septiembre':
    astro_sign = 'Virgo' if (day < 23) else 'libra'
    elif mes == 'octubre':astro_sign = 'Libra' if 
    (day < 23) else 'scorpio'
    elif mes == 'noviembre':astro_sign = 'escorpion' 
    if (day < 22) else 'sagittarius'
    print("tu signo es :",astro_sign)

###### Escriba un programa que calcule el IMC:


    altura = float(input("Tu altura en metros: "))
    peso = float(input("Tu peso en KG: "))
 
    imc = peso / altura**2

    if imc < 16:
	print("desnutricion grave")
    elif imc < 17:
 	print("desnutricion moderada")
    elif imc < 18.5:
	print("delgadez leve")
    elif imc < 25:
	print("normal")
    elif imc < 30:
	print("Sobrepeso")
    elif imc < 35:
	print("obesidad ")
    elif imc < 40:
	print("obesidad severa")
    else:
	print("obesidad grave")


## 3.Bucle while 

###### permite repetir la ejecución de un grupo de instrucciones mientras se cumpla una condición (es decir, mientras la condición tenga el valor True). La ejecución de esta estructura de control while es la siguiente: Python evalúa la condición: si el resultado es True se ejecuta el cuerpo del bucle.

###### Crear un programa que comience en 0 y termine en tu edad.
 
    edad=0
    while edad<19:
        print('tienes',edad)
        edad=edad+1
    print('findeprograma')

###### Crea un programa que te solicite una contraseña para accesar al sistema y en caso de ser incorrecta, te lo notifique y se reinicie utilizando un bucle while.

    llave= 'tesh123'
    while True:
   
    pasword= input('ingrese la contra')
    if pasword==llave:
        print('felicidades entraste al sistem')
        break
    else:
        print('pasword incorrecto ')
        print('favor de intertar de nuevo')

###### Escriba un programa en el que utilizando un bluce while el usuario adivine un numero dado por nosotros ,siguiendo las instrucciones del programa.

    while True:
        numero=int(input('íngresa un numero')
        if numero >=6:
             print(él numero es menor:')
        elif numero <=4:
             print(él numero es mayor')
        elif numero==5:
             print(éres un genio adivinaste')
        else:
             print(íngresa un numero valido')


----
## Bucle for
###### Un bucle for es un bucle que repite el bloque de instrucciones un número prederminado de veces. El bloque de instrucciones que se repite se suele llamar cuerpo  del bucle y cada repetición se suele llamar iteración.

###### Escriba un programa que escriba uno, dos ,tres de forma secuencial utilizando un for;

    secuencia=['uno','dos','tres']
    for elemento in secuencia:
    print(elemento)

###### Escriba un programa que muestre el resultado de la tabla de multiplicar, que el usuario desea obtener.

    n = int(input("que tabla de multiplicar deseas obtener: "))

 
    for i in range(1,11):
       print(n,'x',i,'=',n*i)


###### Escriba un programa que muestre las tablas de multiplicar utilizando un bluce for.


    for i in range(1, 11):
        print("i =", i, ":", end=" ")
    for j in range(1, 11):
        print("{:2d}".format(i * j), end=" ")
    print()

###### Realiza un programa en donde la parte izquierda mueste el precio , mientras que de la parte derecha se muestre el descuento del 60%


    for precio in range(4,200,5):
        precio=precio+0.95
        descuento=precio*60/100
        print(precio,'|',round(descuento,2))


       




## Graficos

###### hay muchos modulos de python que proveen caracteristicas poderosas, que podemos usar en nuestros programas , algunos de estos pueden enviar correos electronicos y tambien pueden extraer informacion de paginas de internet, para el manejo de graficos usaremos un modulo que permite crear figuras y patrones llamado Turtle, permite  desarrollar nuestro pensamiento computacional.

###### Escribe un programa que te pida el color de la ventana y con el modulo turtle dibuje un circulo y lo vaya incrementando al doble.


    print('Escribe uno de los siguiente colores:blue,lightgreen,azure1,azure2,bisque3,brown,aquamarine1,aliceblue,white')

    import turtle
    m=input("ingresa el color de tu ventana:")
    c=int(input('ingresa el numero de vueltas:'))
    k=int(input('ingresa la velocidad:'))
    ventana=turtle.Screen()
    ventana.bgcolor(m)
    ventana.title("Hola, edwin")


    jessie=turtle.Turtle()
     for i in range(c):

     jessie.shape("turtle")
     jessie.color("black")
     jessie.pensize(4)
     jessie.speed(k)
     jessie.penup()
     jessie.setpos(0,-10*i)
     jessie.pendown()
     jessie.circle(10*i)
     ventana.mainloop()

###### Ejemplo este programa nos muestra que para avanzar utilizaremos forward(50) que avanzara 50 unidades y left(120 que girara a la izquierda 120 unidades para finalmente avanzar 50 unidades mas.

    import turtle
    wn = turtle.Screen()
    wn.bgcolor("lightgreen")      
    wn.title("Hello, Tess!")      

    tess = turtle.Turtle()
    tess.color("blue")            
    tess.pensize(3)               

    tess.forward(50)
    tess.left(120)
    tess.forward(50)

    wn.mainloop()


###### Realiza un programa en el que una imagen gif rebote de izquierda a derecha utilizando el modulo turtle.

 
    import turtle
    window= turtle.Screen()
    window.addshape('perro.gif')
    border= turtle.Turtle()
    border.speed(0)
    border.up()
    border.hideturtle()
    border.pensize(5)
    border.color('white')
    border.goto(300,300)
    border.down()
    border.goto(300,-300)
    border.goto(-300,-300)
    border.goto(-300,300)
    border.goto(300,300)


    gato=turtle.Turtle()
    gato.speed(1)
    gato.shape('perro.gif')

    gato.up()
    dx=1

    while True:
    x,y= gato.position()
    if x+dx>=300 or x+dx<=-300:
        dx=-dx
   
    gato.goto(x+dx,y)

    window.mainloop()

    
###### Crear un programa en el que 2 tortugas realicen 2 circulos uno pequeño y uno mas grande.



    print('Escribe uno de los siguiente colores:blue,lightgreen,azure1,azure2,bisque3,brown,aquamarine1,aliceblue,white')
    import turtle
    m=input("ingresa el color de tu ventana:")
    ventana=turtle.Screen()
    ventana.bgcolor(m)
    ventana.title("Hola, jessie")
    jessie=turtle.Turtle()
    jessie.shape("turtle")
    jessie.color("blue")
    jessie.pensize(4)
    mitortuga=turtle.Turtle()
    mitortuga.shape("turtle")
    mitortuga.color("brown")
    mitortuga.pensize(4)
    jessie.speed(1)
    mitortuga.speed(2)
    jessie.penup()
    mitortuga.penup()
    jessie.setpos(0,-50)
    jessie.pendown()
    jessie.circle(50)
    mitortuga.setpos(0,-100)
    mitortuga.pendown()
    mitortuga.circle(100)

    ventana.mainloop()


###### Realiza un programa que pida al usuario que desea graficar(seno,coseno,tangente)Grafique.

     import numpy as np
     import matplotlib.pyplot as plt
     print('Que quieres graficar: 1.seno 2.coseno 3.tangente , elige una opcion')
     op=int(input('escribe tu opcion:'))
     x=np.arange(100)
    if op == 1:
    y=np.sin(x) 
    elif op== 2:
    y=np.cos(x) 
    elif op==3:
    y=np.tan(x)     

    plt.plot(x,y) 
    plt.show()



###### Dibuja un poligono utilizando el modulo turtle.

![image](https://user-images.githubusercontent.com/52517310/60692687-deb4fa00-9e9c-11e9-8e1d-991c7d2a4e1d.png)

    import turtle

    def dibujar_poligono(tur , d):
    for i in range(8):
        tur.forward(d)
        tur.left(45)

    ventana = turtle.Screen()
    ventana.bgcolor('white')
    ventana.title('funciones')

    hush = turtle.Turtle()
    hush.speed(1)
    dibujar_poligono(hush, 50)
    ventana.mainloop


###### Dibuja un cuadro que vaya creciendo de forma secuencial


    import turtle
    ti=turtle.Screen()
    t = turtle.Turtle()
    side = 0
    for i in range(100):
    t.forward(side)
    t.right(90) 
    side = side + 2
    ti.mainloop()


###### Este programa dibuja un remolino utilizando cuadrados , modulo turtle.

![image](https://user-images.githubusercontent.com/52517310/60692715-073cf400-9e9d-11e9-96ac-41a7122b21fd.png)


    import turtle

    def draw_multicolor_square(t, sz):
    
    for i in ["red", "purple", "hotpink", "blue"]:
        t.color(i)
        t.forward(sz)
        t.left(90)

    wn = turtle.Screen()        
    wn.bgcolor("lightgreen")

    tess = turtle.Turtle()      
    tess.pensize(3)

    size = 20                   
    for i in range(15):
    draw_multicolor_square(tess, size)
    size = size + 10        
    tess.forward(10)        
    tess.right(18)          
    wn.mainloop()


###### Dibuja un cuadrado utilizando turtle.

    import turtle

    turtle.forward(50)
    turtle.left(90)
    turtle.forward(50)
    turtle.left(90)
    turtle.forward(50)
    turtle.left(90)
    turtle.forward(50)
    turtle.left(90)

###### El siguiente ejemplo realiza un circulo dibujando cuadrados.

    import turtle
    def draw_square(some_turtle):

    for i in range (1,5):
        some_turtle.forward(200)
        some_turtle.right(90)

    def draw_art():
    window = turtle.Screen()
    window.bgcolor("brown")
    #Turtle Brad
    brad = turtle.Turtle()
    brad.shape("turtle")
    brad.color("white")
    brad.speed(6)
    brad.pensize(2)
    for i in range(1,37):
        draw_square(brad)
        brad.right(10)
    #Turtle Angie
    angie = turtle.Screen()
    angie.shape("turtle")
    angie.color("blue")
    angie.speed(5)
    angie.pensize(2)
    size=1
    while (True):
        angie.forward(size)
        angie.right(91)
        size = size + 1

 
    window.exitonclick()
    draw_art()


###### El siguiente ejemplo muestra como realizar un cuadro creciendo exponencialmente.


    import turtle
    def drawSquare(t,side):
  
    for i in range(4):
  
      t.forward(side)
      t.left(90)


    ventana = turtle.Screen()
    ventana.bgcolor("light green")
    hush = turtle.Turtle()
    hush.fillcolor("red")
    hush.speed(5)

    m = -10


    for s in range(20, 101,20):
   
    drawSquare(hush,s)

    hush.penup()
    hush.goto(m,m)
    hush.pendown()
    m = m -10
  


    ventana.mainloop()


###### El siguiente ejemplo realiza un tiangulo equilatero utilizando turtle.

    import turtle
 
    board = turtle.Turtle()
 
    board.forward(100) # draw base
 
    board.left(120)
    board.forward(100)
 
    board.left(120)
    board.forward(100)
 
    turtle.done()

###### El siguiente ejemplo realiza un rombo utilizando 2 triangulos dibujados con turtle.

    import turtle
 
    board = turtle.Turtle()
 
    board.forward(100) 
 
    board.left(120)
    board.forward(100)
 
    board.left(120)
    board.forward(100)
    board.left(60)
    board.forward(100)
    board.left(120)
    board.forward(100)
 
    turtle.done()


###### En este ejemplo dibujamos pequeños cuadros seguidos de un espacio.

![image](https://user-images.githubusercontent.com/52517310/60692670-d0ff7480-9e9c-11e9-8208-fe92c27093d1.png)


    import turtle

    def dibujar_cuadros_multiples(tur, d):
    for i in range(4):
       
        tur.forward(d)
        tur.left(90)



    ventana= turtle.Screen()
    ventana.bgcolor('lightgreen')
    ventana.title('Funciones')
    hush=turtle.Turtle()
    hush.pensize(4)
    dibujar_cuadros_multiples(hush,20)
    d = 20

    for i in range(16):
    dibujar_cuadros_multiples(hush, d)

    hush.penup()
    hush.forward(50)
    hush.pendown()


    ventana.mainloop()



###### El siguiente programa mueve una imagen de izquierda a derecha en forma de onda.


    import turtle

    window= turtle.Screen()
    window.addshape('nicolas.gif')
    window.bgcolor('lightblue')
    border= turtle.Turtle()
    border.speed(0)
    border.up()
    border.hideturtle()
    border.pensize(5)
    border.color('white')
    border.goto(300,300)
    border.down()
    border.goto(300,-300) 
    border.goto(-300,-300)
    border.goto(-300,300)
    border.goto(300,300)
    sc = turtle.Screen()
    sc.reset()

    sc.setworldcoordinates(0,-1.5,360,1.5)

    for angle in range(360):
    y = math.sin(math.radians(angle))
    fred.goto(angle,y)   

    wn.exitonclick()


    gato=turtle.Turtle()
    gato.speed(1)
    gato.shape('nicolas.gif')

    gato.up()
    dx=1

    while True:
    x,y= gato.position()
    if x+dx>=300 or x+dx<=-300:
        dx=-dx
   
    gato.goto(x+dx,y)

    window.mainloop()


###### El siguiente ejemplo realiza una figura en forma de espiral utilizando cuadros.

![image](https://user-images.githubusercontent.com/52517310/60692698-ed031600-9e9c-11e9-89ae-2bfc0e3dfb3b.png)

    import turtle
    wn = turtle.Screen()
    wn.bgcolor('lightgreen')
    hush = turtle.Turtle()
    hush.pensize(2)
    hush.color('blue')

    def first_two_line(size):
    hush.right(180)
    hush.forward(size)
    hush.right(90)
    hush.forward(size)

    def draw():
    size = 10
    first_two_line(size)
    for i in range(40):
        size += 5
        hush.right(89)
        hush.forward(size)
        hush.right(89)
        hush.forward(size)
    draw()
    wn.mainloop()





## Funciones, Clases Y objetos


## Objeto

###### Un objeto es una identidad que agrupa un estado y una funcionalidad relacionada, el estado del objeto se define a traves de variables llamados atributos, 

mientras que la funcionalidad se modela a taves de funciones a las que se les conoce con el nombre de metodos del objeto.

## clase 

###### clases una clase no es mas que una plantilla general de la cual instancia los objetos es la plantilla que define que atributos y metodos tendran los objetos de esa funcion.

## Sentencia def

###### La sentencia def es una definición de función usada para crear objetos funciones definidas por el usuario. Una definición de función es una sentencia ejecutable. Su ejecución enlaza el nombre de la función en el namespace local actual a un objecto función (un envoltorio alrededor del código ejecutable para la función). Este objeto función contiene una referencia al namespace local global como el namespace global para ser usado cuando la función es llamada. La definición de función no ejecuta el cuerpo de la función; esto es ejecutado solamente cuando la función es llamada.

###### DEFINICION DE UNA FUNCION
    def ladra (num_veces):
    i=0
    while i<num?veces;
    print('gua,gua')
    i=i+1
###### CUERPO PRINCIPAL DEL PROGRAMA
    ladra(5)


###### El siguiente programa calcula el kilometraje que marca un taximetro,despues de 40 km se empieza a cobrar 7.25pesos extra.

    def tarifa(kilometros);
    tarifa=7*kilometros+7.25
    if tarifa<40:
        return 40
    return tarifa
    kilometros=float(input('íngrese su kilometraje')
    precio=tarifa(kilometros)
    print(precio)


###### El siguiente programa calcula es costo de envio y despues de 2 el precio va aumentando.

    def envio(producto):
    envio=(producto-1)*45+150
    return envio

    producto=int(input('íngrese el numero de productos'))
    precio=envio(producto)
    print(precio)


###### en phyton las clases se definen mediante la palabra clave class seguido del nombre de la clase , class automovil y a continuacion.


###### Ejemplo: realiza una clase llamada automovil que lleve los siguientes metodos: arrancar,conducir:


    class Coche(object):
    def __init__(self,gasolina):
       self.gasolina = gasolina
    def arrancar(self):
       if self.gasolina>0:
           print('arrancar')
       else:
           print('no arranca pendejo')
    def conducir(self):
       if self.gasolina>0:
          self.gasolina = self.gasolina - 1
          print('quedan',self.gasolina,'litro')
       else:
           print('no se mueve')

    vocho = vocho(5)
    tsuru = coche(3)
    vocho.arrancar()
    vocho.conducir()
    vocho.conducir()
    vocho.conducir()
    vocho.conducir()
    vocho.conducir()
    vocho.conducir()

###### Realiza una clase llamada triangulo que tenga los siguientes atributos: angulo1,angulo2,angulo3 mitriangulo.


    class triangulo:
    def __init__(self,triangulo1,triangulo2,triangulo3):
        self.angulo1=angulo1
        self.angulo2=angulo2
        self.angulo3=angulo3
    def checar_angulos(self):
        if self.angulo1 + self.angulo2 + self.angulo3== 180:
           print('es verdadero')
        else:
           print('es falso')

    mitriangulo = triangulo(90,30,60)
    mitriangulo.checar_angulos()

###### Realiza una clase llamada letra 

    class letra(object):
    def __init__(self,letra):
        self.letra=letra
    def cantame_una_cansion(self):
       
           print(self.letra)

    micumpleaños=cansion("estas son las mañanitas que cantaba el rey david")
    micumpleaños.cantame_una_cansion()








