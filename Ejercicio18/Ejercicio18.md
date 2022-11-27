# Bibliotecas. Crea una biblioteca dinámica en C que proporcione las funciones para sumar, restar, multiplicar y dividir 2 números enteros. Crea un programa que haga uso de ella y comprueba que se ejecuta correctamente.

Creamos una biblioteca llamada aritmetica con las cuatro operaciones básicas.

1. Compilamos a código objeto dinámico:

~~~
gcc  -c  -fPIC  aritmetica.c
~~~
> Obtendremos el siguiente archivo:

~~~
aritmetica.o
~~~

2. Empaquetamos en biblioteca dinámica `libaritmetica.so` :

~~~
gcc  -shared  -fPIC  -o  libaritmetica.so  aritmetica.o
~~~

Para crear el ejecutable con enlace dinámico:

Creamos el archivo main.c

1. Compilamos y enlazamos, generando un ejecutable `main` y enlace dinámico a `libarimetica.so`

~~~
gcc  -o  main  main.c  libaritmetica.so
~~~

> Obtendremos el siguiente archivo:

~~~
main
~~~

Para ejecutar el archivo `main`, necesitas tener todos los archivos en la misma carpeta y luego ejecutar el comando en la consola:

~~~
./main
~~~

> Obtendremos el siguiente resultado:

~~~
Dados los números 5 y 2
La suma es 7
La resta es 3
La multiplicación es 10
La división es 2.500000
~~~
