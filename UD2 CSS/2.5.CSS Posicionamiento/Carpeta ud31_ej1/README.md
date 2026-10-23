1. Al poner `left: 50px;` en c1 no se mueve, se queda fijo en su valor original

2. Cuadno he puesto `relative con top: 20px y left: 50px.` la caja 2 se ha ido al final y ha salido un poco del contenedor de donde está.

3. Cuando pongo `absolute con top: 0 y right: 0` el cuadro de 3 se va a la esquina derecha de la pagina saliendo del cuadro donde estaba.

4. Cuando a `.contenedor` le doy el valor `position:relative;` el cuadro c3 vuelve dentro del cuadro pero en la esquina derecha.

5. Con el primer cambio de c3 (2.) nadie ocpaba su espacio porque el contenedor se hacia mas pequeño quedandose el el espacio, y en el siguiente cambio(3.) todo se queda igual.