En este proyecto, tuvimos como objeto realizar una pirámide usando solo figuras de ProBuilder. Además, creamos un terreno, le dimos color y añadimos árboles para darle vida
a la escena.


1. Crear la base de la pirámide
<img width="1600" height="858" alt="image" src="https://github.com/user-attachments/assets/a5de6bd3-643e-4908-b877-6f323d11ae5a" />

Comenzamos nuestro proyecto creando una base para la pirámide, este siendo un plano default. El default ya esta dividido en muchas caras lo que nos permite más control sobre la forma, diseño y 
tamaño. Le fuimos haciendo extrude a las caras de los exteriores, pero no las de los bordes, y haciamos extrude mas alto mientras nos acercabamos al centro.


2. Darle forma a la pirámide

<img width="1600" height="844" alt="image" src="https://github.com/user-attachments/assets/67ee7ecc-bf78-4ea7-a086-6e736293851c" />

Primero, le hicimos bevel a las caras pero no nos gusto como quedo. Luego decidimos hacerle extrude a las caras de la esquina hacia abajo, he hicimos extrude a los 
cubos a su alrededos, repetimos esto en cada borde de cada layer hasta llegar hasta arriba. Luego, tomamos unas escaleras de ProBuilder y las agrandamos para que queden
alineadas con la pirámide. Por último, añadimos un plano de 4 caras en el tope de la pirámide que usaremos como piso en el futuro.
 


<img width="1593" height="911" alt="Screenshot 2025-09-24 002323" src="https://github.com/user-attachments/assets/2cf22567-fe24-4e7b-95e3-ec7233e3395c" />
3. Crear mini estructuras

Para crear estas estructuras se usaron dos planos para cada una. Tomamos un plano default de ProBuilder, y le hicimos merge a las caras para formar 3 paredes
y una entrada, y le hicimos extrude. Para hacer el hueco de la entrada le hicimos extrude horizontalmente a la cara desde la derecha. Para la parte negra adentro
de la estructura, se le hizo extrude a dos caras adentro y se pintaron de negro usando el material TerrainLit. Usamos otro plano y lo colocamos arriba para el techo, 
esencialmente fue jugar con las caras hasta encontrar un diseño que nos gustara, pero la idea fue merge las caras del interior, merge y todas las demas caras hicieron la forma.
Por ultimo, hicimos merge las caras del exterior que sirven como plataforma.



4. Darle color al proyecto
<img width="1861" height="1006" alt="Screenshot 2025-09-24 010418" src="https://github.com/user-attachments/assets/b9feccc0-8eb4-404e-a4d0-600de91c354b" />

Primero empezamos con darle color a los mini templos. Primero, creamos dos materiales bajo assets, uno para el color azul y otro para rojo. Para colorear la plataforma de los templos,
ya habiamos hecho merge las caras, entonces lo que hicimos fue detach todas las caras merged como otro GameObject (después aprendimos que podemos usar submesh, y no se crea otro objeto), y
le dimos color. Para el techo como era un plano entero, solamente le dimos color. Entonces, para darle color a la pirámide, creamos otro material para el color marrón, y tuvimos que ir 
layer por layer merging todas las caras de ese layer, para hacerles detach como submesh y darles el color marrón a cada layer. Para la escalera, inicialmente teniamos solamente una pero la 
dividimos en 3 partes, 2 menos anchas a los exteriores y la del medio siendo mas larga, a esta le dimos color marrón. Por último, hicimos un material nuevo para el color blanco, y simplemente
se lo aplicamos al plano entero de la pirámide, ya que todo lo que le dimos color marrón estaba separado, y a las escaleras.


5. Crear el terreno y decorar
<img width="1350" height="665" alt="image" src="https://github.com/user-attachments/assets/66371fb5-5f3d-4b91-ae9c-f2d7c09c57e6" />


Para crear el terreno, primero tuvimos que download un asset para terrenos llamado: Terrain Sample Asset Pack. Tomamos la brocha "builtin_brush_6" en brush size 165 y 50 opacity. 
Queríamos darle un estilo de "mossy area, mossy rocky area" (como el ejemplo), entonces los terrain layers que usamos fueron: Muddy_Terrain, Heather_Terrain, Rock_Terrain y Soil_Rocks_Terrain. Fuimos poco a poco
pintando hasta encontrar un buen ambiente de donde puede ser que este un templo escondido. Decidimos revaluar los colores de la pirámide y decidimos que era mejor cambiarlos, por eso, descargamos un asset llamado FreeConcreteMaterials y reemplazamos el blanco por concrete.
