# LAB4-API-HILOS

## (a) Nombres completos de los integrantes, correos y números de documento.

### Santiago Jiménez Escobar - santiago.jimeneze@udea.edu.co - C.C 1036959331
### Emiro Moreno Soto - emiro.morenos@udea.edu.co - C.C 1001547311

## (b) Documentación de todas las funciones desarrolladas en el código.

## 2. Generador de Secuencia de Fibonacci
El programa utiliza un hilo trabajador para calcular la secuencia de Fibonacci y almacenarla en un arreglo compartido reservado dinámicamente por el hilo principal.

La comunicación entre el hilo principal y el hilo trabajador se realiza mediante una estructura **(`DatosFib`)** que contiene el valor de **`N`** y un puntero al arreglo compartido.

El hilo principal utiliza **`pthread_join()`** para sincronizar la ejecución y garantizar que la secuencia haya sido calculada completamente antes de imprimir los resultados.

El uso de memoria compartida evita copias innecesarias de datos y permite que el hilo trabajador escriba directamente en el arreglo que posteriormente será leído por el hilo principal.
![wgrep](capturas/CodFibonacci1.png)
![wgrep](capturas/CodFibonacci2.png)
![wgrep](capturas/CodFibonacciResultado.png)



## (c) Problemas presentados durante el desarrollo de la practica y sus soluciones.


## (d) Pruebas realizadas a los programas que verificaron su funcionalidad.

En la siguiente imagen se observa la ejecución del programa base y su resultado
![wish](capturas/mem_map2.PNG)


## (e) Un enlace a un video de 10 minutos donde se sustente el desarrollo.

[Haz clic aquí para ver el video](https://youtu.be/TeelQA6-_2Y)


## (f) Manifiesto de transparencia: En que puntos se apoyaron de la IA generativa.

## (g) Al menos cinco conclusiones.

## (h) Notebook de analisis.
