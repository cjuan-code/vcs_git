## Ejercicio de Sistemas de Control de Versiones

Para este ejercicio he decidido utilizar la metodología GitHub Flow, explicación:

<ul>
  <li> Todo lo que se desplega en lo que se encuentra en la rama master (rama de producción)</li>
  <li> Para añadir una característica nueva, se crea una rama con un nombre distintivo de la funcionalidad a implementar</li>
  <li> Se realiza el commit en local y se hace un push con el mismo en el server </li>
  <li> Una vez revisado el código, ya podemos mergear contra master </li>
  <li> Una vez mergeado, debemos desplegar los cambios </li>
</ul>

Como todo, tiene sus ventajas y desventajas

Ventajas: 
<ul>
  <li> Se recomiendo para features de duración corta (diarias o incluso de horas) </li>
  <li> Flujo ligero y recomendado si el proyecto requiere de una entrega de valor constante </li>
</ul>

Desventajas: 
<ul>
  <li> Inestabilidad de master si no se utilizan las herramientas de testing/PR correctamente. </li>
  <li> No recomendado para múltiples entornos productivos. </li>
  <li> Dependiendo del producto, podemos tener restricciones de despliegues. </li>
</ul>

Primero haremos las clonaciones para la simulación del trabajo en equipo.
![1](https://user-images.githubusercontent.com/79716922/135763778-ec1e2de4-c1ac-4a1d-ae1b-ebab82d690f6.png)

### Usuario 1

Ahora, el usuario1 creará la estructura inicial de los ficheros utilizando la metodología elegida. La página principal se ve así:

![2](https://user-images.githubusercontent.com/79716922/135763779-2b623a30-2de1-4430-bac6-289d51fbf4cb.png)

Una vez realizada toda la estructura, el usuario1 commiteará todos los cambios.

![3](https://user-images.githubusercontent.com/79716922/135763781-37593200-21e5-410c-97f0-1852bbf6bacb.png)

y procederá a hacer el push al repositorio de GitHub.

![4](https://user-images.githubusercontent.com/79716922/135763782-6fa7fcde-3880-4370-b2d1-87fb3fbcff09.png)


### Usuario 2

El usuario2 se ocupará de realizar 2 features, contenidoHTML y atributosHTML. Primero se actualizará realizando un git pull y creara una rama nueva.

![5](https://user-images.githubusercontent.com/79716922/135763783-15688215-5d30-4da6-a1b8-5306d0011bb3.png)

La feature de contenidoHTML se ve de la siguiente manera:

![6](https://user-images.githubusercontent.com/79716922/135763784-b7a91123-883c-49c6-97b0-f2986f20b0ed.png)

Una vez realizada la feature realizará un commit.

![7](https://user-images.githubusercontent.com/79716922/135764192-43057d5e-f91a-4362-9a68-2f7f0adbbf20.png)

Ahora procederá a realizar la feature de atributosHTML, creando una nueva rama de nuevo.

![8](https://user-images.githubusercontent.com/79716922/135763786-b126d54b-e41f-465b-9e99-0531f3cfabc6.png)

La feature de atributosHTML se ve de la siguiente manera:

![9](https://user-images.githubusercontent.com/79716922/135763787-7f86312b-3163-4cb7-802b-678629ff23a9.png)





