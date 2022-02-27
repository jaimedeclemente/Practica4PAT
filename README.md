# Practica4PAT
## Conexión a una API financiera

En esta práctica, hemos mejorado las funcionalidades del apartado de Cotización de la web insertando datos de la misma gracias a una API financiera.

### Navegación:
Al igual que en la práctica anterior, al abrir la página, le saldrá un *disclaimer* explicando que la página no es la oficial de la compañía. Éste le aparecerá únicamente la primera vez que abra la página. 

En la pantalla principal, tendrá algo de información sobre la empresa en el *body*, un link en el logo del *footer* así como ciertos datos de la empresa y su localización y, finalmente, tres botones en el *header*. Cada uno de esos botones le llevará a diferentes páginas con más información.

Dándole al primero de ellos, **Quiénes Somos**, llegará a una explicación del funcionamiento de la empresa, sendas tablas con los conformantes de su Consejo de Administración y su Equipo Directivo y, finalmente, un formulario que, en un futuro, serviría para apuntarse a la *newsletter* de la empresa. 

Pinchando en **Activos**, llegará a una explicación de los diferentes sectores de inmuebles que tiene la empresa. Navegando a cada uno de ellos, podrá ver tablas con ejemplos de los mismos. 

Pulsando en **Cotización** accederá al desempeño en bolsa de la empresa en tiempo real gracias a un *iframe* de una página de análisis bursátil. Además, como se explica en el siguiente apartado, se ha introducido una tabla con los datos más significativos del desempeño en bolsa en el último día de cotización.

*Cabe destacar, para facilitar la navegación, que siempre que se encuentre en cualquier ventana diferente a la principal podrá volver a esta última pulsando en el logo existente en el *header* de la página correspondiente.*

### Cambios:
Así, nos hemos conectado a la API para conseguir la información de la **Apertura**, el **Cierre**, la **Variación** y el **Volumen** conseguido por la acción en el último día en el mercado. Estos datos, una vez procesados desde el JSON que nos devuelve la API, han sido insertados en la web dentro de una tabla, situada encima del *iframe* que nos muestra la gráfica de la cotización.

Por lo demás, la web ha permanecido igual a como estaba en la última práctica.

El código necesario para realizar la conexión a la API y la inserción de los datos en el HTML se incluye en el archivo *cotizacion.js*.

**PD:** *El archivo que sería la página principal de la web se llama index.html*
