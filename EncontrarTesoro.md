# Ejercicio Encontrar el Tesoro

procedimiento EncontrarTesoro(){
    /*PROPÓSITO: El pirata debe recorrer el camino marcado hasta llegar al tesoro. A medida que avanza puede ser que el pirata se tope con una muralla, en ese caso debe derribarla pintandola de color negro. El pirata comineza un paso previo al inicio del camino.
    PRECONDICIÓN: El pirata debe recorrer al menos 19 parcelas hacía el este y 6 parcelas hacía el norte a partir del inicio del pirata.*/

        IrAlPrimerTramo()
        repetir 2 veces {
            TramoEste()
            TramoNorte()
        }
}

procedimiento IrAlPrimerTramo(){
    /*PROPÓSITO: El pirata debe moverse de su parcela actual hacía el inicio del camino.
    PRECONDICIÓN: Debe haber al menos 1 parcelas hacia el este a partir del inicio del pirata.*/

        MoverDerecha
}

procedimiento TramoEste(){
    /*PROPÓSITO: El pirata debe recorrer el tramo revisando en cada parcela si es que hay alguna muralla y en ese caso derribarla. Inicia en la celda actual.
    PRECONDICIÓN: Debe haber al menos 6 parcelas hacía el este a partir de la celda actual.

        si (estaPintadaDeRoja?) entonces {
            DerribarMuralla()
        }
        repetir 6 veces {
            MoverDerecha
            si (estaPintadaDeRoja?) entonces {
                DerribarMuralla()
            }
        }
}

procedimiento TramoNorte(){
    /*PROPÓSITO: El pirata debe recorrer el tramo revisando en cada parcela si es que hay alguna muralla y en ese caso derribarla. Inicia en la celda actual.
    PRECONDICIÓN: Debe haber al menos 3 parcelas hacía el norte a partir de la celda actual.

        repetir 2 veces {
            MoverArriba
            si (estaPintadaDeRoja?) entonces {
                DerribarMuralla()
            }
        }
        MoverArriba
}

procedimiento DerribarMuralla(){
    /*PROPÓSITO: Cuando el pirata se encuentre una muralla debe derribarla, para esto debe pintarla de color negro. inicia en la celda actual.
    PPRECONDICIÓN: Se necesita minimo una parcela.

        Limpiar
        PintarNegro
}