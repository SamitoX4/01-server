<!-- Instalaciones para crear servidor -->

  <!-- Paquete para crear el servidor express -->
  npm install express

  <!-- Paquete para permitir servir recursos restringidos desde otro sitio -->
  npm install cors

  <!-- Paquete que sirve para transformar el cuerpo de las solicitudes a un formato -->
  <!-- mas entendible o procesable -->
  npm install body-parser

<!-- Luego se tiene que inicializar el archivo de configuracion de TS -->
tsc --init

  <!-- En este archivo tener en cuenta lo siguinte -->

  "module": Especificar qué código de módulo se genera
  "outDir": Especifica una carpeta de salida para todos los archivos emitidos

  <!-- Nota: Tener en cuenta que el modulo CommonJS es necesario para el uso -->
  <!--       en el backend cuando se utiliza NodeJS y express por otro lado -->
  <!--       si estas usando NestJS, deberias utilizar ES6 o afines. -->
  <!--       Con respecto a angular seria otro tema. Investigar! -->

<!-- Para probar esto vamos a utilizar dos cosas -->

  <!-- Poniendo a mirar los cambios de los archivos -->
  <!-- Si algun archivo se guarda o cambia algo, esto -->
  <!-- lo detecta -->
  tsc -w

  <!-- Poniendo a mirar lo que se compila en la carpeta -->
  <!-- "dist" que seria la carpeta outDir del archivo tsconfig.json -->
  <!-- puedes configurar otra carpeta si es necesario -->
  nodemon dist/