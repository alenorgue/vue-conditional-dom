# Ejercicios con forumularios y Vue


Abre con Live Server cada uno de los ficheros index.html del ejercicio a ralizar

En alguno de ellos tendrás que [configurar el HTML](https://vuejs.org/guide/quick-start.html#using-the-global-build) para quea gobernado por Vue 


## ¿Algo va mal?


0. Intenta no pedir la solución directa a la IA.
1. Asegurate de que has hecho bien el [setup]((https://vuejs.org/guide/quick-start.html#using-the-global-build)) , engoblado todo el HTML por un contenedor `<div id="app"></div>` 
2. Echa un vistazo a la consola del navegador. Normalmente sucede que nos olvidamos importar algo o hay un error de sintaxis
<img src="https://oscarm.tinytake.com/media/17910d3?filename=1753086794204_TinyTake21-07-2025-10-33-00_638886835924646084.png&sub_type=thumbnail_preview&type=attachment&width=615&height=486" title="Powered by TinyTake Screen Capture"/>

### 0-sant-feliu-guixols-rocks

Disponemos de un selector para obtener información sobre la ciudad de Sant Feliu de Guíxols. Lo que sucede es que ahora mismo nos aparece toda la información _de golpe_ , y queremos seleccionar lo qué mostrar.

Usa adecuadamente las directivas [v-if...v-else-if...](https://vuejs.org/guide/essentials/conditional#v-if) para mostrar una sección u otra. ¡Fíjate en el valor del atribute _value_ de cada una de las opciones del select!

**Tan solo debes modificar el HTML para conseguir esto...*** ¡Fíjate en el valor de la variable de estado!


### 1-rock-paper-scissors

Este juego de piedra papel tijeras ya está implementado y funcionando correctamente.
El problema, es que aparecen los mensajes de que ¡has ganado! y ¡has perdido! todo el tiempo.

Usa adecuadamente las directivas [v-if...v-else-if...](https://vuejs.org/guide/essentials/conditional#v-if) para mostrar solo el HTML correcto cuando el jugador ha ganado 3 rondas o la IA ha ganado 3 rondas.

**BONUS**: Usa adecuadamente la directiva v-if o [v-show](https://vuejs.org/guide/essentials/conditional#v-show) para ocultar el panel de juego una vez ha finalizado.

**Tan solo debes modificar el HTML para conseguir esto...** ¡Fíjate en el valor de las variables de estado!

### 2-registration-form

Crea un formulario típico de registro. Este formulario tiene varias peculiaridades:

1. Debido a que queremos aprovechar la validación de los formularios (el campo required, que un texto sea un email, etc); hemos usado el tag <form>. 
2. Entonces, no usaremos el evento _click_ para gestionar el formulario, si no el evento [_submit_](https://vuejs.org/guide/essentials/event-handling.html#event-modifiers)
3. Solamente tras hacer clic en el checkbox "I accept the terms of use", aparece el botón de submit
4. Cuando el formulario valida y todos los datos son correctos, se oculta el contenedor del formulario y aparece otro explicando los datos que ha enviado el usuario.


<details>
  <summary>Pista 1: Comprueba una posible configuración de variables de estado</summary>
  <pre>
    const name = ref('') // nombre
    const age = ref('') // edad
    const email = ref('') // email
    const accepted = ref(false) // el checkbox de aceptar las condiciones
    const submitted = ref(false) // si ya ha enviado el formulario o no
  </pre>
</details>



