# Lenguaje C++. Código en varios archivos. Obtener el código objeto y binario a partir del código fuente de los 3 archivos siguientes:

> Para obtener el código objeto ejecutamos el siguiente comando:

~~~
g++ -c main.cpp datos.cpp suma.cpp
~~~

- Obtendremos los siguientes archivos:

~~~
datos.o main.o suma.o
~~~

> Para obtener el código binario ejecutamos el siguiente comando:

~~~
g++ -o programa main.o datos.o suma.o
~~~

- Obtendremos el binario ejecutable:

~~~
programa
~~~

Para ejecutar el programa debemos ejecutar el siguiente código:

~~~
./programa
~~~



