# Ejercicio 3: Dibujar Flecha

    **Utilizando QDraw, escribir un programa, con su correspondiente documentación, que dibuje la flecha que se muestra en la imagen. El cabezal inicia en la celda central de la punta de la flecha.**

programa {
    /* PROPÓSITO: Dibujar una flecha en diagonal descendente a la derecha. Plumas rojas, tallo negro y punta verde. El cabezal inicia en la pluma izquierda y termina en la esquina superior de la punta de la flecha.
    PRECONDICIÓN: Se necesita al menos una celda hacía arriba, 4 celdas a la derecha y 3 celdas hacía abajo.
    */

            DibujarPlumas()
            IrAExtSupDeTalloDeFlecha()
            DibujarTallo
            IrAExtInfIzqDePuntaDeFlecha()
            DibujarPuntaDeFlecha()

}

procedimiento DibujarPlumas(){
    /* PROPÓSITO: Dibujar dos plumas rojas. El cabezal inicia en la pluma izquierda y termina en la pluma derecha. 
    PRECONDICIÓN: Se necesita al menos una celda hacía arriba y una celda a la derecha.
    */

            PintarRojo
            MoverArriba
            MoverDerecha
            PintarRojo

}

procedimiento IrAExtSupDeTalloDeFlecha(){
    /* PROPÓSITO: Ir de la posición actual al extremo superior del tallo de la flecha. 
    PRECONDICIÓN: Se necesita al menos 1 celda hacía abajo.
    */

            MoverAbajo

}

procedimiento DibujarTallo() {
    /* PROPÓSITO: Dibujar el tallo de la flecha de color negro. El cabezal comineza en la posición actaul y termina en el extremo inferior de la flecha.  
    PRECONDICIÓN: Se necesitan al menos 2 celdas hacía la derecha y 2 celdas hacía abajo a partir de la posición inicial del cabezal.
    */

            repetir 2 veces {
                PintarNegro
                MoverAbajo
                MoverDerecha
            }
            PintarNegro

}

procedimiento IrAExtInfIzqDePuntaDeFlecha() {
    /* PROPÓSITO: ir del tallo de la fleha al extremo inferior izquierda de la punta de la flecha. 
    PRECONDICIÓN: Se necesita al menos 2 celdas a la izquierda y una hacía abajo.
    */

            MoverAbajo
            MoverIzquierda

}

procedimiento DibujarPuntaDeFlecha() {
    /* PROPÓSITO: Dibujar la punta de la flecha de color verde. El cabezal inicia en la posición actual y termina en el extremo superior derecho de la flecha. 
    PRECONDICIÓN: Se necesitan al menos 2 celdas a la derecha y 2 hacía arriba a partir de la posición inicial del cabezal.
    */

            DibujarExtInfIzq()
            MoverDerecha
            DibujarPunta()
            MoverArriba
            DibujarExtSupDer()

}

procedimiento DibujarExtInfIzq() {
    /* PROPÓSITO: Dibujar el Extremo Inferior Izquierdo de la punta de la flecha de color verde. El cabezal inicia en la posición actual y termina una celda a la derecha.  
    PRECONDICIÓN: Se necesita al menos 2 celdas a la derecha a partir de la posición inicial de la flecha.
    */

            PintarVerde
            MoverDerecha
            PintarVerde

}

pocedimiento PintarPunta() {
    /* PROPÓSITO: Dibujar punta de la flecha de color verde. Inicia en la posición actual. 
    PRECONDICIÓN: Se necesita el espacio de la celda actual.
    */

            PintarVerde

}

procedimiento DibujarExtSupDer() {
    /* PROPÓSITO: Dibujar el Extremo superior derecho de la punta de la flecha de color verde. El cabezal inicia en la posición actual y termina una celda hacía arriba.  
    PRECONDICIÓN: Se necesita al menos 2 celdas hacía arriba partir de la posición inicial de la flecha.
    */

            PintarVerde
            MoverArriba
            PintarVerde

}