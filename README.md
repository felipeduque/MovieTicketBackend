# MovieTicketBackend
Back


Esquema y estructura de la aplicación de Reservas HotelTicketBackend
Aplicación de reserva de Hoteles que almacenaba todos los datos de la película en archivos javascript. Eso obviamente no es lo que quieres hacer para una aplicación del mundo real. Por lo tanto, esta vez vamos a construir un backend API para nuestra aplicación de reserva de Hoteles  que almacenará datos de Hoteles en una base de datos MongoDB y lo devolverá a la aplicación como datos JSON.
Requisitos previos
MongoDB
Para instalar la aplicación de terminal ejecutar MongoDB:

Npm install mongodb
Ahora, creemos una carpeta que MongoDB usará para almacenar nuestra base de datos:

sudo mkdir -p / data / db
Y establece los permisos correctos:

sudo chmod 777 / data / db
Finalmente, vamos a lanzar MongoDB:

Mongod&
Inicializar el proyecto Node.js
crea una nueva carpeta:
mkdir MovieTicketsBackend;
cd MovieTicketsBackend;
npm init
Eso creará el archivo package.json que se utiliza para almacenar la información, los scripts y las dependencias de su aplicación.

Instalar dependencias
instale las dependencias de desarrollo que necesitaremos durante el desarrollo y ejecute la aplicación localmente:

npm install --save-dev babel babel-cli babel-preset-es2015 babel-preset-stage-0 nodemon
Y luego, instala todo el resto:

npm instalar --save body-parser express moment mongoose morgan
Crear archivo .babelrc
Crea un nuevo archivo llamado .babelrc con el siguiente contenido:
{
  "presets": ["es2015", "stage-0"]
} 
Eso nos permitirá usar las características de JavaScript de ES6 a las que tenemos acceso cuando desarrollemos HotelTickets. En el caso de React Native, ES6 está habilitado por defecto.
