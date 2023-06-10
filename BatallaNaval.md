# Ejercicio Batalla Naval.

procedimiento EliminarBarcosDelOceano() {
    /*PROPÓSITO: Retirar del juego tanto barcos chicos como grandes, colocando agua en su lugar. El cabezal inicia en la esquina inferior izquierda y termina en la esquina inferior derecha.
    PRECONDICIÓN: Debe haber al menos 7 celdas hacia arriba y 7 hacia la derecha a partir del inicio del cabezal.*/

            repetir 3 veces {
            RecorrerCaminoArribaBarcos()
            MoverHaciaOtroCamino()
            RecorrerCaminoAbajoBarcos()
            MoverHaciaOtroCamino()
            }
            RecorrerCaminoArribaBarcos()
            MoverHaciaOtroCamino()
            RecorrerCaminoAbajoBarcos()

}

procedimento RecorrerCaminoArribaBarcos() {
    */PROPÓSITO: Recorrer el camino eliminando los barcos chicos y grandes si es que hay alguno, para esto colocar agua en su lugar pintando de negro. Comineza en la celda actual.
    PRECONDICIÓN: Se necesita al menos 7 celdas hacia arriba a partir de la celda actual.*/

            repetir 7 veces {
            si (estaPintadaDeRojo? v estaPintadaDeVerde?) entonces {
                Limpiar
                PintarNegro
            }
            MoverArriba
            }
            si (estaPintadaDeRojo? v estaPintadaDeVerde?) entonces {
                Limpiar
                PintarNegro
            } 

}

procedimiento MoverHaciaOtroCamino() {
    /*PROPÓSITO: Mover el cabezal de un camino a otro. Inicia en la celda actual.
    PRECONDICIÓN: Debe haber al menos 1 celda a la derecha a partir de la celda actual.*/

            MoverDerecha

}

procedimento RecorrerCaminoArribaBarcos() {
    */PROPÓSITO: Recorrer el camino eliminando los barcos si es que hay alguno, para esto colocar agua en su lugar pintando de negro. Comineza en la celda actual.
    PRECONDICIÓN: Se necesita al menos 7 celdas hacia abajo a partir de la celda actual.*/

            repetir 7 veces {
                si (estaPintadaDeRojo? v estaPintadaDeVerde?) entonces {
                Limpiar
                PintarNegro
                }
                MoverAbajo
            }
            si (estaPintadaDeRojo? v estaPintadaDeVerde?) entonces {
                Limpiar
                PintarNegro
            }

}

/--------------------------------------------------------------------------------------------/

procedimiento MarcarOceano() {
    /*PROPÓSITO: Despinta todas las celdas que representan agua. Inicia en la esquina inferior izquierda y termina en la esquina inferior derecha.
    PRECONDICIÓN: Debe haber al menos 7 celdas hacia arriba y 7 hacia la derecha a partir del inicio del cabezal.*/

            repetir 3 veces {
                RecorrerCaminoArribaAgua()
                MoverHaciaOtroCamino()
                RecorrerCaminoAbajoAgua()
                MoverHaciaOtroCamino()
            }
            RecorrerCaminoArribaAgua()
            MoverHaciaOtroCamino()
            RecorrerCaminoAbajoAgua()

}

procedimento RecorrerCaminoArribaAgua() {
    */PROPÓSITO: Recorrer el camino eliminando las celdas que representan agua. Comineza en la celda actual.
    PRECONDICIÓN: Se necesita al menos 7 celdas hacia arriba a partir de la celda actual.*/

            repetir 7 veces {
                si (estaPintadaDeNegro?) entonces {
                    Limpiar
                }
                MoverArriba
            }
            si (estaPintadaDeNegro?) entonces {
                Limpiar
            }        

}

procedimento RecorrerCaminoAajoAgua() {
    */PROPÓSITO: Recorrer el camino eliminando las celdas que representan agua. Comineza en la celda actual.
    PRECONDICIÓN: Se necesita al menos 7 celdas hacia arriba a partir de la celda actual.*/

            repetir 7 veces {
                si (estaPintadaDeNegro?) entonces {
                    Limpiar
                }
                MoverAbajo
            }
            si (estaPintadaDeNegro?) entonces {
                Limpiar
            }        

}