# notas-sobre-sailsjs
trucos y notas sobre sailsjs

# Para corregir el error `sails.config.orm._hookTimeout'
agregar la sigiente linea en /config/env.development.js
  hookTimeout: 60000

#DEPLOYAR LA APP
Agregar la siguiente linea a la tarea de grunt uglify
  options: {
      mangle: false
  },
