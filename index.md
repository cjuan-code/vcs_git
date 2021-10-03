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

Ahora mergeará la rama estilosCSS, como podemos ver, también hay conflicto, por lo que el usuario1 lo resolverá manualmente de nuevo y posteriormente realizará el commit y push al repositorio.

![19](https://user-images.githubusercontent.com/79716922/135763801-dd054b0e-eb05-4ed9-a584-097062c1df1e.png)

Una vez mergeado todas las features, creará un tag "v1.0" y lo subirá al repositorio.

![20](https://user-images.githubusercontent.com/79716922/135763802-23f104a9-3604-4d9b-ad6d-aaf7ae116143.png)

Ahora creará una rama de testing para que los testers de la empresa prueben la aplicación.

![21](https://user-images.githubusercontent.com/79716922/135763804-bf97ac03-839e-4938-a43e-03090b32f221.png)

#### Automatización

El usuario1 se encargará de realizar los hooks para automatizar algunas funciones. Primero creará el hook para que cada vez que se realize un cambio de rama, los paquetes se actualizarán automáticamente.

![22](https://user-images.githubusercontent.com/79716922/135763805-7efa8701-5e40-4e20-b584-1943627b3424.png)

Aqui podemos ver su funcionamiento.

![comp_hook_checkout](https://user-images.githubusercontent.com/79716922/135763810-ef085524-d208-48b3-ae93-702422eb333a.png)

Ahora creará el hook para la verificación de los commits.

![23](https://user-images.githubusercontent.com/79716922/135763806-f6a1b8a6-c3a5-4894-bb52-39170dfc15fa.png)

Aqui podemos ver el funcionamiento de este.

![comp_hook_commit_msg](https://user-images.githubusercontent.com/79716922/135763811-c5b17394-5544-42f6-a5a4-5dfcb0c8215f.png)

También comprobará que antes de que se realize un push verifique que ninguno de los fichero contenga caracteres extraños.

![24](https://user-images.githubusercontent.com/79716922/135763807-ff782760-d8e2-4f28-b703-3124f6f4b461.png)

Este es su funcionamiento.

![comp_hook_pre_push](https://user-images.githubusercontent.com/79716922/135763813-61b16582-b38a-4601-9070-cb40d7e523ec.png)

Y por último, se verificará el formato correcto de los ficheros .html antes de realizar un commit, utilizando un [eslinter](https://www.npmjs.com/package/eslint-plugin-html).

![25](https://user-images.githubusercontent.com/79716922/135763808-d1d8bae9-6e49-43fa-9a43-2bf4a0582aaf.png)

Este es su funcionamiento.

![comp_hook_pre_commit](https://user-images.githubusercontent.com/79716922/135763812-83c72bc4-dc10-4f02-bfe4-69d180b6b1c8.png)

Una vez solucionado los errorres, se realizará el último push.

![solucion_eslinter](https://user-images.githubusercontent.com/79716922/135763815-67d90390-b887-47c4-ac4d-4fde4c1b766d.png)

Todos los hooks realizados se encontrarán el la carpeta gitHooks/ para que todos los usuarios puedan acceder a ellos.
