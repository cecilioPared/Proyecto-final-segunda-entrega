# Proyecto-final-segunda-entrega

Segunda entrega proyecto final programación backEnd

## Configuración inicial

Previo a la ejecución del proyecto se debe crear en el directorio raiz del mismo un archivo `.env` con 2 variables 
```
NODE_PORT=8080
NODE_ENV=local
FIREBASE_PATH=../utils/proyectofinal-firebase-admin.json
PERSISTENCIA=json```

Los valores configurables en la variable de entorno `PERSISTENCIA` son:

  json -> para implementación en archivos
  mongodb -> para implementación en mongodb atlas
  firebasedb -> para implementación en base de datos fierbase
  y por default para implementación en memoria
  
Una vez configuradas las variables de entorno se debe ejecutar el siguiente comando para inicializar la aplicación

```
npm run dev
```

## Permiso de usuario

Se utiliza un parametro en la cabecera de la llamada al endpoint `key:role` - `value:admin` el cual se controla en un middleware de validación llamado validarUsuarioAdminMiddleware.

## Postman

En el directorio raiz del proyecto se encuentra un archivo de colección  `Proyecto-final-segunda-entrega.postman_collection.json` con las configuraciones para poder probar los endpoint de la API. El mismo se debe importar desde postman.  

## Archivo Config

Este archivo posee las configuraciones de conexion a mongo atlas y el path donde se generan los archivos de colecciones para carrito y productos
