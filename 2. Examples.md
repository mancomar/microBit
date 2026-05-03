Variables  
```
#Con este programa cramos un contador de pulsaciones con una variable llamada counter
from microbit import *

counter = 0

while True:
    if button_a.was_pressed():
        counter += 1
        if counter > 10:
            counter = 0
        display.scroll(str(counter))
```
Bucle If

```
from microbit import *
import random

numbers = ["orange", "yellow", "green", "blue"]

while True:
    if button_a.was_pressed():
        display.scroll(numbers[random.randint(0, 3)])

```
