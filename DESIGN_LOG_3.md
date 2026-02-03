# Actividad 3: Micro-interacciones y Feedback al Crear Rutas

## Decisiones de diseño

Darle una retroalimentación al usuario mientras cargan los eventos es de suma importancia porque el usuario puede entrar en pánico e intentar repetir sus acciones, terminando comúnmente en fallos en el sistema y duplicados. Por eso, ahora se implementó un sistema de toast para notificar al usuario lo que está sucediendo para que pueda estar tranquilo. Con ayuda de Tailwind es muy sencillo hacer toasts con un diseño normalizado.

* Clic: Ahora al hacer clic en cualquier parte del mapa, se abre un formulario emergente (popup) limpio y estilizado.

* Toast: Se implementó un sistema de alertas visuales.

* Cargando: Muestra un spinner animado cuando guardas.

* Éxito: Muestra una confirmación verde cuando se completa el guardado.

* Marcadores Dinámicos: Los nuevos restaurantes se agregan al mapa usando un icono por default de utensilios.

* Lógica: Todo ocurre sin recargar la página, manteniendo la fluidez y dinamismo de la app.

## Prompts de Gemini Canvas

* "Ahora quiero añadir la funcionalidad de agregar un nuevo restaurante. Quiero que cuando el usuario le di clic al mapa, se cree un puntero y en un popup salga un mensaje que diga "Nombre del restaurante" y una caja de texto para escribir el nombre, debajo otro texto para ingresar una breve descripción del restaurante y su respectiva caja de texto, y más abajo un botón de guardar. Después de darle al botón de guardar, debe aparecer un toast con animación para indicarle al usuario que está cargando su solicitud (simular 1 segundo de carga) y después mostrar otro toast con un mensaje de éxito. Después de esto, el marcador debe aparecer en el mapa con un icono de utencilios de comida como el "fa-utensils" de font-awesome. Todo esto debe seguir la paleta de colores que ya está establecida."
* "Ahora sólo quiero que me ayudes a reubicar los toast porque aparecen en medio de la pantalla y sobrepuestos en el header y no se ve bien. Quiero que se muestren del lado izquiero con unos 10px de separación del borde de la pantalla y otros 10px de separación con el header para que no esté encimado. También noté que el popup del marcador que carga al inicio de "Tacos" tiene un diseño difente al que se crea junto con los nuevos marcadores. Quiero que se unifique todo con el diseño de los nuevos marcadores, pero sin la leyenda de "Agregado recientemente" porque es redundante.".