# Parcial 1. Ejercicio 2.

Un laboratorio nos ha solicitado automatizar el mantenimiento de los tubos de ensayo de su sala principal. Se sabe que la sala cuenta con 3 mesas con cubículos 1x1 donde se encuentran los tubos de ensayo. Hay un solo tubo por cubículo. Cada mesa cuenta con un total de 50 cunículos.
Para esta tarea, contamos con la robot Labby que deberá mantener todas las mesas con tubos sanos en base a la siguiente representación de la información:
- celdas vacías: representan los cubículos sin tubos.
- Celdas rojas: representa los cubículos con tubos rotos.
- Celdas verdes: representa los cubículos con tubos sanos.
- Celdas negras: representan los bordes de la mesa. Cada uno mide 1x1 metro2.
Se solicita definir el procedimiento *ReemplazarTubosDeSala()*, en el cual Labby deberá reemplazar, de las 3 mesas de la sala del laboratorio, cada tubo de ensayo roto por uno sano. Es decir que al finalizar la tarea, las mesas no deberán contener cubículos con tubos rotos.
Labby inicia en el cubículo inferior izquierdo de la primer mesa.
