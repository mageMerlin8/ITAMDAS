# ITAMDAS
##### Propuesta Emilio Mena Garcia

La idea general es desarrollar una aplicación que funcione como cuenta de débito para los estudiantes del itam que además
busque fomentar el ahorro de sus usuarios. También se busca implementar una cadena de bloques (blockchain) como capa extra
de seguridad y de trazabilidad.

Se conceptualiza el proyecto en 3 etapas generales.

### Etapa 1 - Prototipo

En la primera etapa se desarrolla un prototipo útil y se desplega a un ambiente muy parecido al ambiente productivo final.
El 'producto' en esta etapa se piensa como un sistema de cuentas de débito. Aunque no sea el producto entero, se puede
pensar en el sistema de cuentas de débito como el sistema operativo del producto final y por lo tanto será el enfoque de
esta primera etapa.

Como parte del 'sistema operativo' del producto se desarrollará un sistema para guardar las transacciones en una cadena
de bloques (blockchain) auto administrada por [AWS](https://aws.amazon.com) llamada [Amazon QLDB](https://aws.amazon.com/es/qldb/).

Se utilizará PHP como lenguaje backend principal y la aplicación se desarrollará sobre Laravel [framework](https://laravel.com).
Se eligen estas tecnologías por su facilidad, su buena documentación y la experiencia del equipo de desarrollo.

Para esta etapa la aplicación se montará en [Heroku](https://heroku.com). Heroku es un proveedor de nube como servicio
(PaaS), es muy accesible e incluye un plan gratuito. El plan gratuito es suficiente para las pruebas de esta etapa. Además
Heroku tiene la capacidad para escalar a millones de usuarios por lo que no sería necesario mover la aplicación a otro
proveedor cuando iniciemos pruebas más pesadas.

Entregables:

    [  ] Esquema de base de datos
    [  ] APIs para compartir información entre la BD y la aplicación
    [  ] API para guardar las transacciones en Amazon QLDB
    [  ] Aplicación web/progresiva

------------------------
### Etapa 2 - Desarrollo del Producto y UX

Durante la segunda etapa contempla el desarrollo del producto como tal. Se personaliza, se le da una marca y un proposito.
Durante esta etapa la aplicación se debería estar probando por algunas personas (no todos parte del equipo de
desarrollo) sin dinero real para medir el desempeño real.

Durante esta etapa se deben definir las ventajas competitivas del producto y estas deben ser desrrolladas como funcionalidades
de la aplicación. El 'feature' de tandas se debe aterrizar y desarrollar. Además se busca mejorar la estética de la aplicación.

Por otro lado, las pruebas técnicas de la plataforma deben continuar. En esta etapa se busca el uso por 5-10 usuarios
cercanos al equipo para identificar errores y mejoras. Cabe recalcar que esto debe ser un proceso que se repita continuamente
a través de la vida de la aplicación.

----------------------------
### Etapa 3 - Introducción del Producto en el Mercado

Durante la tercera etapa se abre la apliacación al público con todo lo que esto implica. Lo más importante y dificil de esta
etapa tiene que ver con el manejo de dinero.

El principal obstaculo en esta última etapa es el manejo del dinero. Hasta ahora, la aplicación no mueve dinero de verdad.
Es necesario un lugar en donde guardar los fondos, un método para fondear las cuentas de los usuarios y un métdo para
que los usuarios puedan disponer del dinero que tengan en sus cuentas.



------------------------------

