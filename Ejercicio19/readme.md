# Bibliotecas. Crea una biblioteca dinámica en Java que proporciona las funciones para sumar, restar, multiplicar y dividir 2 números enteros. Crea un programa que haga uso de ella y comprueba que se ejecuta correctamente.

 Creamos el directorio `aritmetica` 

~~~
mkdir aritmetica
~~~

1. Creamos la clase `aritmetica.java`

2. Compilamos con el siguiente comando:

~~~
javac  aritmetica/Aritmetica.java
~~~

> Obtendremos un archivo `aritmetica,java`con el bytecode.

3. Creamos el paquete jar con el siguiente comando:

~~~
jar  cvf  aritmetica.jar  aritmetica/*.class
~~~

> Obtendremos un archivo `aritmetica.jar`

Para ejecutar el archivo tenemos que descargar los archivos en la misma carpeta y ejecutar el siguiente comando: 

~~~
java   -jar    aritmetica.jar
~~~


