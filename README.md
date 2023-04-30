**Primera Entrega de mi Proyecto Final👩‍💻**

De acuerdo a la consigna de pre entrega, este trabajo contiene:

1. Algoritmos condicionales
2. Algoritmos utilizando un ciclo
3. Armado de un simulador interactivo de acuerdo a la estructura final de proyecto integrador
4. Utilización de funciones para llevar a acabo algoritmos sencillos

Formato

Página HTML y código fuente en JS

1. Archivo JS referenciado en el HTML por la etiqueta  <scriptsrc="miarchivo.js">`</script>`

### Diseño y estilos del simulador interactivo

El diseño de este trabajo utiliza el framework Bootstrap. Lo que permite que sea un diseño de página web responsive.


# Explicación del desarrollo de simulador interactivo

Hasta el momento se han realizado dos funciones en JavaScript:

01-calcularCostoTotal()

02-agregarMas()

En cuanto a la función 01 permite calcular el costo total de un pedido de pan mediante el ingreso de tipo de pan y cantidad, mediante prompts, en dónde el cliente o usuario añade lo que desea.

### ¿Qué utiliza la función 01?

Esta función utiliza un bucle while que permite el ingreso de productos y cantidades, y el bucle finaliza hasta que el usuario decide finalizar la compra. Se puede resumir la función en el siguiente algoritmo paso a paso:

1. La función definida como calcularCostoTotal() utiliza la sintaxis de función flecha.
2. La variable de tipo boolena 'finalizado' se declara como false para indicar que el bucle no ha terminado.
3. El bucle while que inicia solo se ejecutará mientras finalizado sea false.
4. Se utilizan prompts para solicitar el ingreso de datos como pan y cantidad.
5. En la variable producto se guardan los datos solicitados en prompt.
6. Si el cliente o usuario da click en cancelar en la ventana del prompt se establece 'finalizado' como true.
7. Se utiliza la palabra reservada continue para saltar al siguiente ciclo del bucle.
8. Si ingresa un nombre de pan válido, se solicita la cantidad empleando ParseInt y se guarda el dato en la variable cantidad
9. Las variables costo y costoProducto inician su valor en 0.
10. Se utiliza la sentencia switch para  determinar el precio de costoProducto según el nombre del pan en este caso puedes ingresar como válidos "baguette, batard, boule, bagel, pizza".
11. Si el cliente ingresa el nombre de un pan que no está en la lista, manda un mensaje en alerta para que ingrese un producto válido, se utiliza continue para saltar a la última parte del bucle
12. Si la cantidad de panes ingresada es mayor a 0 se calcula el costo multiplicando costoProducto * cantidad, se muestra un alert con el resultado.
13. El bucle se repite hasta que el usuario decida presionar el botón de cancelar, una vez finalizada la compra, la función termina de ejecutarse.

    ### ¿Qué utiliza la función 02?

    En cuanto a la función 02 esta pensada para clientes que recién ya hicieron un pedido y para saber si quieren agregar algo más, esta función permite añadir productos a un pedido, una compra o en otra situación a un carrito de compras, este algoritmo funciona así paso a paso:


    1. La variable 'continuar' se inicializa en si y se solicita mediante prompts al usuario que agregue el primer producto a su pedido.
    2. El bucle while se ejecutará mientras la respuesta del usuario sea si o sí (acentuado) en cuanto a si desea agregar más productos.
    3. Dentro del bucle el usuario podrá responder si desea agregar más productos o panes a su pedido o compra, si la respuesta es si o sí se pedirá el nombre del pan a agregar
    4. Si el usuario o cliente responde 'no' o algo distinto a 'si' o 'sí' el bucle termina y se imprime un alert de agradecimiento por su compra
