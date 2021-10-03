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

Una vez realizada la feature realizará otro commit.

![10](https://user-images.githubusercontent.com/79716922/135763788-7e4d58ac-12b7-4eaa-af29-8c9c3d566e3e.png)

Una vez finalizadas las features, realizará los push de las ramas al repositorio.

![11](https://user-images.githubusercontent.com/79716922/135763789-8eca5be4-66c9-47ec-a74e-e74ac7f906de.png)
![12](https://user-images.githubusercontent.com/79716922/135763791-195f03c8-b15d-4e5f-81ca-0c1c248c9c87.png)

### Usuario 3

El usuario3 se ocupará de realizar la feature de estilosCSS creando una rama nueva.

![13](https://user-images.githubusercontent.com/79716922/135763792-b93cdc0a-d8f7-4986-945e-4b28e589f8f2.png)

La feature se ve así:

![14](https://user-images.githubusercontent.com/79716922/135763793-f648fb70-a683-42f4-876a-757da81c327f.png)

Una vez hecha, realizará el commit y el push al repositorio.

![15](https://user-images.githubusercontent.com/79716922/135763795-f7e7a31f-53c2-463d-8a27-4f2d9702e115.png)

### Usuario 1

Ahora que ya están todas las features realizadas, el usuario1 se actualizara haciendo un git pull.

![16](https://user-images.githubusercontent.com/79716922/135763796-288f95f0-4531-4535-8770-342bb0dbe095.png)

También se encargará de mergear las features a la rama master. En la siguiente captura, se puede ver que ha habido un error al hacer el git merge, por tanto, el usuario1 lo resolverá manualmente.

![17](https://user-images.githubusercontent.com/79716922/135763798-f7ca66ba-8819-44b6-a434-2e57a82ad681.png)

Una vez resuelto el conflicto, realizará un commit de los merge de las features contenidoHTML y atributosHTML realizadas por el usuario2.

![18](https://user-images.githubusercontent.com/79716922/135763800-39c8f2d8-6535-4e04-a10b-b5e3ba3231c8.png)

Ahora mergeará la rama estilosCSS, como podemos ver, también conflicto, por lo que el usuario1 lo resolverá manualmente de nuevo.

![19](https://user-images.githubusercontent.com/79716922/135763801-dd054b0e-eb05-4ed9-a584-097062c1df1e.png)


