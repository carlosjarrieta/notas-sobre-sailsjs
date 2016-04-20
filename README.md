### notas-sobre-sailsjs
trucos y notas sobre sailsjs

### Para corregir el error `sails.config.orm._hookTimeout'
agregar la sigiente linea en /config/env.development.js <br/>
    **hookTimeout: 60000**

### DEPLOYAR LA APP
    Agregar la siguiente linea a la tarea de grunt uglify
    options: {
      mangle: false
    },

###2) config/local.js

In your Sailsconfig (config/local.js) you have to set Host, Port and Environment. See **local.js**. 
Example:

    host: process.env.OPENSHIFT_NODEJS_IP || "127.0.0.1",
    port: process.env.OPENSHIFT_NODEJS_PORT || 8080,
    environment: process.env.NODE_ENV || 'development'
