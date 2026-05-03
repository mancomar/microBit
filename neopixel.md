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
