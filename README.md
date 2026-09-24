# Comandero

Comandero móvil para el camarero de una cafetería. Sirve para anotar rápido lo que piden los clientes de cada mesa, marcharlo a barra y cobrarlo.

Es un único archivo, `index.html`, sin dependencias ni paso de compilación. Solo carga las fuentes de Google Fonts.

## Qué hace

- **Sala**: mesas por zonas (Sala, Terraza, Barra). Las ocupadas muestran el importe pendiente, el tiempo abierta y lo que falta por marchar.
- **Tomar nota**: un toque en un producto suma una unidad. Si mantienes pulsado o activas «✎ Con nota», se añade con notas rápidas (sin lactosa, corto, en vaso…) o con texto libre.
- **Marchar**: marca lo que ya se ha pedido a barra.
- **Suplemento de terraza**: cada producto puede llevar su propio suplemento. Se aplica en las zonas que lo tengan activado y se recalcula al pasar un pedido de una mesa a otra.
- **Cobrar**: en efectivo, con cálculo del cambio, o con tarjeta. Se puede **dividir la cuenta** por artículos o a partes iguales.
- **Caja**: lo cobrado en el día (efectivo, tarjeta, ticket medio, lo más pedido) y el detalle de cada ticket, con días anteriores.
- **Carta**: aquí se editan productos, precios, suplementos, notas rápidas, mesas y zonas.

## Usarla

Abre `index.html` en el navegador del móvil. Para tenerla en una dirección web, activa **GitHub Pages** en el repositorio: *Settings → Pages → Deploy from a branch → `main` / root*. Después, desde el navegador del móvil, elige «Añadir a pantalla de inicio».

## Dónde se guardan los datos

- **Abierta desde GitHub Pages o como archivo**: todo se guarda en el propio navegador (`localStorage`). Cada móvil tiene sus propios datos, y si borras los datos del navegador, se pierden.
- **Abierta como Artifact en claude.ai**: usa la base de datos compartida del artifact. Todos los camareros ven las mismas mesas en tiempo real.

La app detecta sola en qué modo está. Arriba a la derecha indica «Compartido» o «Solo este dispositivo».
