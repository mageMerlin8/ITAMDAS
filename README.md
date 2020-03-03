# PROYECTO - ITANDA

El propósito del proyecto es brindar a los integrantes de la comunidad ITAM una Plataforma Interuniversitaria de Cobros 
y Pagos Digitales que facilite las transacciones monetarias que se realizan día a día. En la actualidad diversas Fintech 
ofrecen servicios similares, sin embargo, buscamos innovar el mercado agregando nuevas opciones que incentiven la cultura 
del ahorro y bienestar de las finanzas personales.

La plataforma contará con las siguientes opciones:

 - Opciones para cobrar/pagar, ya sea a través del número de cuenta de un usuario específico o con tecnología Quick Response.
 - Opciones para establecer metas de ahorro, con la posibilidad de automatizar la extracción de montos por periodos de tiempo.
 - Opciones para formar parte de sistemas de ahorro compartido. Esto con el objetivo de estudiar el comportamiento de pago
  de los usuarios y que se puedan brindar créditos, etc.
 - La mayor innovación del proyecto es que la estructura de datos que se va a implementar para realizar el registro 
 de las transacciones de los usuarios es una cadena de bloques (blockchain). Esto brindará mayor seguridad y trazabilidad a la plataforma.

----------------------------------------------------

Se conceptualiza el proyecto en 3 etapas generales.

### Etapa 1 - Prototipo

En la primera etapa se desarrolla un prototipo útil y se despliega en un ambiente muy parecido al ambiente productivo 
final. El 'producto' en esta etapa se piensa como un sistema de cuentas de débito. Aunque no sea el producto entero, 
se puede pensar en el sistema de cuentas de débito como el sistema operativo del producto final y por lo tanto, será 
el enfoque de esta primera etapa.

Como parte del 'sistema operativo' del producto se desarrollará un sistema para guardar las transacciones en una cadena
 de bloques (blockchain) auto administrada por AWS llamada Amazon QLDB.

Se utilizará PHP como lenguaje backend principal y la aplicación se desarrollará sobre Laravel framework. Se eligen estas 
tecnologías por su facilidad, su buena documentación y la experiencia del equipo de desarrollo.

Para esta etapa la aplicación se montará en Heroku. Heroku es un proveedor de nube como servicio (PaaS), es muy accesible
e incluye un plan gratuito. El plan gratuito es suficiente para las pruebas de esta etapa. Además Heroku tiene la 
capacidad para escalar a millones de usuarios por lo que no sería necesario mover la aplicación a otro proveedor cuando
iniciemos pruebas más pesadas.

Entregables:

    [  ] Esquema de base de datos
    [  ] APIs para compartir información entre la BD y la aplicación
    [  ] API para guardar las transacciones en Amazon QLDB
    [  ] Aplicación web/progresiva
 
 -------------------------------
### Etapa 2 - Desarrollo del Producto y UX
La segunda etapa contempla el desarrollo del producto como tal. Se personaliza, se le da una marca y un propósito. Durante esta etapa la aplicación debería de ser probada por diferentes personas (no todos parte del equipo de desarrollo) sin dinero real para medir el desempeño.
Durante esta etapa se deben definir las ventajas competitivas del producto y estas deben ser desarrolladas como funcionalidades de la aplicación. El 'feature' de tandas se debe aterrizar y desarrollar. Además se busca mejorar la estética de la aplicación. Se debe contemplar el desarrollo de una aplicación blockchain sobre un marco existente en la nube como el ofrecimiento de IBM de managed Blockchain que utiliza el marco Hyper Ledger.
Por otro lado, las pruebas técnicas de la plataforma deben continuar. En esta etapa se busca el uso por 5-10 usuarios cercanos al equipo para identificar errores y mejoras. Cabe recalcar que esto debe ser un proceso que se repita continuamente a través de la vida de la aplicación.
El final de esta etapa o el inicio de la siguiente es el momento óptimo para cambiar de proveedor de nube si así lo desea el equipo. El cambio se haría hacia uno de los proveedores más grandes como AWS y Google. Esto nos permitiría reducir los costos de operación.

-----------------------------------
### Etapa 3 - Introducción del Producto en el Mercado
Durante la tercera etapa se abre la aplicación al público con todo lo que esto implica. Lo más importante y difícil de esta etapa tiene que ver con el manejo de dinero.
El principal obstáculo en esta última etapa es el manejo del dinero. Hasta ahora, la aplicación no mueve dinero de verdad. Es necesario un lugar en donde guardar los fondos, un método para fondear las cuentas de los usuarios y un método para que los usuarios puedan disponer del dinero que tengan en sus cuentas.


