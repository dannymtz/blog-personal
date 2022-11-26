## Heroku ##

Este blog esta desplegado dentro de [Heroku](https://www.heroku.com/) con el beneficio 
de tener un server bajo demanda o como se le conoce "Serverless" esta tecnologia 
nos brinda una bajo costo ya que solo esta activo cuando es requerido, 
en este post muestro el paso a paso para poder tener un proyecto desplegado en heroku. 

Este proyecto esta compuesto por el proyecto de codigo abierto
[gitbook](https://www.npmjs.com/package/gitbook) desarrollado bajo la tecnologia de node.

Solo me centrare en explicar el despliegue dentro de Heroku para la documentación
de descarga y uso de gitbook favor de consultar mi post de gitbook.

Se requiere instalar en la terminal Heroku CLI
* Descargar de su portal para desarrolladores [https://devcenter.heroku.com/articles/heroku-cli](https://devcenter.heroku.com/articles/heroku-cli)

Una vez descargada la consola y registrados en Heroku procedemos a loguearnos en la consola
con el comando 

``heroku login``

Para el siguiente paso, mi recomendación es tener tu proyecto en control de versiones
en mi caso estoy ocupando github donde igual podras encontrar mi codigo de este post.

```
git add . 
git commit -am "nuevo proyecto o cambios"
git push heroku master
```
En caso de tener un repositorio de un proyecto 

````
heroku git:remote -a test-proyecto-muestra
````