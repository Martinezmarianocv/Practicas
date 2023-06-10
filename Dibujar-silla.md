# Ejercicio 2: Dibujar Silla.

    a. Utilizando QDraw, escribir un programa, con su correspondiente documentación, que dibuje la silla que se muestra en la imagen. El cabezal se encuentra en la parte inferior de la pata delantera de la silla.

programa {
    /* PROPÓSITO:Dibujar una silla de color negro. El cabezal inica en la parte inferior de la pata delantera de la silla y termina en la parte superior del respaldo de la silla.
    PRECONDICIÓN:Se necesitan al menos 3 celdas hacía la izquierda y 5 celdas hacía la arriba a partir de la posición inicial del cabezal.
    */

            DibujarPata()
            MoverArriba()
            DibujarAsiento()
            IrAPataTrasera()
            DibujarPata()
            IrArriba()
            DibujarRespaldo()

}

procedimiento DibujarPata(){
    /* PROPÓSITO:Dibujar una pata de la silla de color negro. El cabezal inicia en la posición actual y termina en la celda superior a la inicial. 
    PRECONDICIÓN:Se necesita al menos una celda hacía arriba a partir de la posición inicial del cabezal.
    */

            pintarNegro
            MoverArriba
            PintarNegro

}

procedimietno MoverArriba() {
    /* PROPÓSITO: Mover el cabezal una celda hacía arriba a partir de la posición actual del cabezal.
    PRECONDICIÓN:Se necestia al menos una celda hacía arriba a partir de la posición actual del cabezal.
    */

            MoverArriba

}

procedimiento DibujarAsiento() {
    /* PROPÓSITO: Dibujar el asiento de la silla de color negro. el cabezal inicia en la posición actual y termina en el extremo trasero del asiento.
    PRECONDICIÓN:Se necesita al menos 2 celdas hacía la izquierda a partir de la posición inicial del cabezal.
    */

            repetir 2 veces {
                PintarNegro
                MoverIzquierda
            }
            PintarNegro

}
procedimiento IrAPataTrasera(){
    /* PROPÓSITO: Mover el cabezal desde la posición actual hasta el extremo inferior de la pata trasera.
    PRECONDICIÓN: Se necesita al menos 2 celdas hacía abajo y una hacía la izquierda a partir de la posición inicial del cabezal.
    */

            repetir 2 veces {
                MoverAbajo
            }
            MoverIzquierda

}

proccedimiento DibujarRespaldo(){
    /* PROPÓSITO:Dibujar el respaldo de la silla de color negro. El cabezal inicia en la posición actual y termina en el extremo superior del respaldo. 
    PRECONDICIÓN:Se necesitan al menos 3 celdas hacía arriba a partir de la posición inicial del cabezal.
    */

            repetir 3 veces {
                PintarNegro
                MoverArriba
            }
            PintarNegro

}


    b. Si tuviéramos la siguiente imagen con el cabezal iniciando en otra celda. ¿Qué cambiaría?

progrma {
    /* PROPÓSITO:Dibujar una silla de color negro. El cabezal inica en la parte inferior de la pata trasera de la silla y termina en la parte superior del respaldo de la silla.
    PRECONDICIÓN:Se necesitan al menos 3 celdas hacía la derecha y 5 celdas hacía la arriba a partir de la posición inicial del cabezal.
    */

            MoverAPataDelantera()
            DibujarPata()
            MoverArriba()
            DibujarAsiento()
            IrAPataTrasera()
            DibujarPata()
            IrArriba()
            DibujarRespaldo()

}