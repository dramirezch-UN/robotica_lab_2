# Robótica - Laboratorio 2

Este laboratorio fue una continuación del trabajo realizado en el primer laboratorio, en el cual se propone crear dos entradas y dos salidas digitales configurándolas correctamente en el código de RAPID. La primera señal de entrada debe iniciar una rutina de escritura sobre cualquier superficie y encender una luz de indicación. Al final de la rutina, el brazo debe regresar a su posición de HOME donde todos los ángulos articulares son 0 grados. La segunda señal de entrada debe posicionar el brazo en una pose de mantenimiento donde se pueda instalar o desinstalar la herramienta y se debe apagar la luz de indicación.

## Programación en Robot Studio
Inicialmente, basados en el trabajo del anterior laboratorio, se programaron en Robot Studio las dos rutinas (escritura y mantenimiento).
![rutinas](https://i.imgur.com/hr1vR9z.png)

Después, se agregaron las entradas y salidas digitales dentro del simulador por medio de la interfaz I/O System e I/O Simulator. Estas se ubicaron en su posición dentro de la rutina y se realizaron las simulaciones para confirmar su correcto funcionamiento.

![io](https://i.imgur.com/xn4D29W.png)

Por último, se exportó el código RAPID para su montaje en el laboratorio.

## Montaje Final
En el laboratorio se realizó el cableado correspondiente entre el panel de pulsadores y el controlador para los dos pulsadores y un testigo. Un problema que se encontró en el desarrollo del laboratorio fue que el robot se encontraba descalibrado y al intentar correr el código, este se bloqueaba. Con ayuda del docente se pudo calibrar y continuar con el desarrollo. Se realizaron ciertas modificaciones en el Flex Pendant, se cambiaron los moveL de la rutina de mantenimiento a moveJ, lo cual permitió obtener un movimiento más fluido, esto también como recomendación del profesor.
![montaje](https://i.imgur.com/T7mYGY2.png)
