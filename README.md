# Localizador SII

Aplicacion web estatica y minimalista para consultar informacion de propiedades y terrenos en Chile, obteniendo datos directos del Servicio de Impuestos Internos (SII) sin necesidad de utilizar su interfaz oficial.

## Caracteristicas

- Busqueda simplificada: Solo necesitas ingresar la Comuna, la Manzana y el Predio (ROL de la propiedad).
- Mapeo automatico: Traduce el nombre de la comuna ingresada por el usuario al codigo interno utilizado por la API del gobierno.
- Extraccion de coordenadas: Muestra las coordenadas del terreno tanto en formato Grados, Minutos, Segundos (DMS) como en formato Decimal.
- Generacion de enlaces: Crea un enlace directo para abrir la ubicacion exacta en Google Maps.
- Datos financieros: Extrae de forma automatica el catastro valorizado, desglosando el avaluo total, exento y afecto en formato CLP.
- Interfaz moderna: Diseno purista, modo oscuro nativo, responsivo y adaptado completamente para uso en dispositivos moviles (celulares y tablets).
- Copiado rapido: Botones integrados para copiar bloques enteros de informacion o datos individuales directamente al portapapeles.

## Tecnologias utilizadas

El proyecto esta construido 100% en el lado del cliente (Frontend), lo que permite que sea hosteado en cualquier servicio estatico sin requerir un servidor backend.

- HTML5
- CSS3 (Variables nativas, animaciones y CSS Grid/Flexbox)
- JavaScript Vanilla (Fetch API y Clipboard API)

## Como utilizar

1. Ingresa a la pagina principal alojada en GitHub Pages.
2. En el primer campo, escribe el nombre de la comuna de la propiedad. Aparecera una lista de sugerencias.
3. En los campos posteriores ingresa la manzana y el predio.
4. Presiona el boton de busqueda. Si el ROL existe en la base de datos oficial y cuenta con registros geograficos, la informacion se desplegara en segundos.

## Deployment

Este proyecto esta disenado para funcionar directamente sobre GitHub Pages. Al no tener dependencias de backend como Node.js o Python, basta con subir el archivo `index.html` a la rama principal de un repositorio para que este completamente funcional y accesible en internet.
