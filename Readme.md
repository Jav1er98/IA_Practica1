## Práctica 1: Múltiples tipos de agente persiguiendo al jugador.
## Modifica el proyecto "Agentes en el Nav Mesh" para incluir un First Person Controller, de forma que tres tipos distintos de agente persigan al jugador. Crea tipos de agentes con propiedades diferentes para que se generen NavMeshes diferentes para cada tipo (como hicimos en el proyecto "Múltiples NavMesh para distintos tamaños de agente"), de forma que tengan que buscar caminos alternativos para perseguir al jugador.

En primer lugar llevamos a cabo el desarrollo de un First Person Controller que se le incorpora al objeto Player. A este objeto le añadimos un Character Controller y un script para controlar el movimiento. 

Nuestros agentes serán 3 capsulas de diferentes colores, en este caso rojo, azul y verde, a cada una de estas capsulas les añadimos el script proporcionado en clase denominado "Chase Player" para que persigan por el mapa al jugador, a su vez añadimos al mapa el script "NavMeshSurface" tres veces, una para cada agente, en la pestaña navigation añadiremos los bakes para cada agente y luego se los asignaremos a cada objeto en su correspondiente "Nav Mesh Agent".

Una vez ajustado cada Navmesh el resultado que nos queda es el siguiente:

![Paso 1](gifs/Captura1.png)
![Paso 2](gifs/Captura2.png)
![Paso 3](gifs/Captura3.png)
![Paso 4](gifs/Captura4.png)
      
Si observamos con atención el ajuste de cada agente, se presentarán los siguientes casos:
 -  El azul es demasiado alto por lo cual no podrá seguir al jugador.
      ![Paso 5](gifs/gif1.gif)
      
 -  El rojo es demasiado ancho, tendrá que coger otro camino que habilitamos, mientras que el verde puede seguir al jugador por donde quiera.
      ![Paso 6](gifs/gif2.gif)
      
      ![Paso 7](gifs/gif3.gif)
