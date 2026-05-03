Si usamos como editor Mu, podemos comprobar errores luego de compilarlo en Micro:bit activando el botón REPL (Read-Eval-Print-Loop).
En este ejemplo de programa vamos a programar un pixel del tipo Neopixel, en este caso solo tiene un diodo.  
Con Neopixel(pinxx. n) indicamos el pin al que conectamos el Neopixel y el núemro de diodos, con np[i]=(256,256,256) indicamos el pin que queremos encender y con qué color.  

```
# Escribe tu código aquí :-)
from microbit import *
import neopixel

# Inicializamos la tira NeoPixel en el pin0 con 8 LEDs
# Ajusta el '8' al número de LEDs que tenga tu tira o anillo
np = neopixel.NeoPixel(pin8, 1)

while True:
    # Encendemos el primer LED (posición 0) de color rojo
    np[0] = (100, 8, 55)
    np.show()
    sleep(1000) # Espera 1 segundo
    # Apagamos todos los LEDs
    np.clear()
    np.show()
    sleep(1000)
    while ( pin16.read_digital() == 0 ):
        for i in range(0, 255, 10):
            for j in range (0, 255, 10):
                for k in range (0, 25, 10):
                    np[0] = (i, j, k)
                    np.show()
                    np.clear()
                    sleep(100)
```
    
