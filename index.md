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
![1](https://user-images.githubusercontent.com/79716922/135763361-f8058d8a-2634-422d-871a-1ca6a6e3d471.png)


