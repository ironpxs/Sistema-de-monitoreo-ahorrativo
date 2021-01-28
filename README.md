# Sistema de monitoreo ahorrativo
Sistema de control de luces y monitoreo con ahorro energético para conjuntos residenciales.
### Integrantes:
1. Asanza Romero Claudia Sofía 
2. Choez Espinoza Elvis Joel 
3. Choez Villacis Steven Ariel 
4. Herrera Nieto Homar Flavio 
5. Paz Castro Alejandro Emanuel
6. Pita Elias Juan Xavier

### Planteamiento del problema
En el conjunto residencial La Joya en la etapa Zafiro, el administrador desea implementar un sistema de monitoreo con luces incluidas, debido a que el consumo de luz es excesivamente alto al tener que estar las luces prendidas toda la noche para que personas y animales no estén en el club social en horas no permitidas. Para esto el administrador ha solicitado el desarrollo de un circuito en el cual las luces enciendan en la noche y cuando exista un clima nublado con poca luminosidad, el sistema de monitoreo únicamente estará activo en la noche y cuando existe algún movimiento, finalmente se solicita que el diseño posea un modo de ahorro de energía.

### Solución del problema

Como desarrolladores planteamos un circuito en el cual las luces se enciendan o se apagan mediante:

- Reloj digital R, el cual indicara si es noche mediante la señal R=1.
- Indicador de luz ambiental L implementado mediante una fotocelda, si se encuentra L=1 indica que aún existe luz ambiental.

Asimismo, el sistema de monitoreo se enciende o apaga:

- Sensor de movimiento que permite detectar si movimiento, M = 1 indica que si existe un
movimiento en el área.

Por último, para ahorrar energía se implementarán 2 switchs, que permiten el ahorro de energía en el estado (AB=11). Si uno se encuentra encendido las luces o sistema de monitorio podría o no encenderse, dependiendo de L, para las luces se implementa un dimmer programable para atenuar la luz de acuerdo con el requerimiento del usuario y el nivel de ahorro de energía que desee, y dependiendo de R para el monitoreo, además si en cierto tiempo no se detecta movimiento este se apaga.

### Funciones con don't cares minimizadas mediante mapas de Karnaugh
F1 = A'L' + B'R
F2 = A'R M

### Circuito en Proteus
