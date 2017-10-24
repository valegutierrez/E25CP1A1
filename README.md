# Experiencia 25 - Actividad Presencial I
## CRUD AJAXEABLE

El objetivo de esta actividad es aprender a implementar AJAX en un CRUD generado mediante scaffold.

#### Para realizar esta actividad debes haber visto los videos correspondientes a la semana 25.

## Ejercicio 1:

#### Primera Parte:

- Crear un nuevo proyecto en Rails 5.1

- Crear un scaffold de Post que contenga sólo el campo título.
- El formulario de creación de un nuevo Post debe ser implementado en el index.
- Al agregar un nuevo Post, este debe ser añadido al listado del index de Post de manera dinámica, es decir, el formulario debe ser enviado por AJAX, el controlador almacena el recurso y la respuesta en JS debe agregar el nuevo elemento al listado.
	> Hint: El nuevo recurso debe ser agregado a la lista mediante el método de jQuery **.append()**

- Al eliminar un Post este debe ser eliminado de manera dinámica, es decir, el borrado debe ser enviado mediante AJAX, el controlador elmina el recurso y la respuesta en JS debe remover el elemento del listado.
	> Hint: Para el borrado, se recomienda agregar un id correspondiente al id del Post a cada tag **\<tr>** a cada Post listado en la tabla y luego utilizar el método de jQuery **.toggle()**

- Se debe integrar un buscador de Post que, mediante AJAX, debe arrojar resultados de manera dinámica a medida que se va escribiendo en el input de texto.
	> Hint: El buscador debe comenzar a arrojar resultados a partir del ingreso de 3 caracteres en adelante.

#### Segunda Parte:

- Agregar la gema Carrierwave.

- Agregar un campo al modelo Post y montar un uploader en él.

-  El formulario de creación de un nuevo Post debe recibir una imagen local.
	> Hint: Para poder subir archivos a formularios que son enviados mediante AJAX revisa la gema [remotipart](https://github.com/JangoSteve/remotipart).

#### Bonus:
- El formulario de edición debe ser levantado en un modal que al ser enviado debe cerrar el modal y mostrar el contenido actualizado en el listado del Index de Post.
