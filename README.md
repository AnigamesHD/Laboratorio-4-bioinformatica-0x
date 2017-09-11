# Laboratorio-4-bioinformatica-0x

# Nombre: Byron Guzmán Marín

## Plataforma phylogeny.fr y preparación de datos

__¿Qué cosas ofrece este portal?__

 El portal Phylogeny.fr, conecta varios programas de bioinformática para reconstruir árboles filogenéticos desde un conjunto de secuencias. Entre lo que ofrece la página, es posible realizar análisis filogenéticos de tres formas distintas (“One Click”, “Advanced” y “A la Carte”), donde cada modo tiene un orden de opciones de las cuales el investigador puede seleccionar. Además, es posible realizar un análisis con BLAST sobre una secuencia, para explorar secuencias homólogas que se encuentren en la base de datos. Por otra parte, el portal además entrega vínculos de acceso a programas online en la página principal, para alineamientos múltiples, filogenia, visualización de árboles filogenéticos, entre otras herramientas útiles. 
 
 __¿Para qué tipo de usuario está diseñado?__
 
La idea central del portal Phylogeny.fr es asistir y proveer con las herramientas necesarias a biólogos sin experiencia en filogenia, para que sea posible analizar su información de un modo robusto, con fuentes de información comprensibles y flexibles.

__Menciona 5 tipos de análsis que se pueden realizar en el portal de acuerdo a la documentación__

Análisis del alineamiento, por medio del programa MUSCLE; refinamiento del alineamiento, mediante Gblocks, donde el programa elimina posiciones alineadas de forma pobre y regiones divergentes; análisis de la filogenia, por medio del programa PhyML; y representación del árbol, a través del programa TreeDyn, donde se muestra la imagen final del árbol obtenido mediante las secuencias colocadas, que puede ser luego editado según el interés del usuario. Otro tipo de análisis es mediante BLAST, para explorar secuencias homólogas a la secuencia que se desee analizar, donde el sistema facilita la selección de estas mediante una representación filogenética y un estimador del largo del alineamiento.

## Inferencia de genomas

# Filogenia inferida con parámetros: ProbCons (Alineamiento), GBlocks (Alignment curation), MrBayes (Filogenia), y TreeDyn (representación del árbol):

https://www.dropbox.com/s/j302w0u5kfbev0x/foto%201.jpg?dl=0

https://www.dropbox.com/s/zd7f99ehv1wdxe9/phylo_tree.pdf?dl=0

# Filogenia inferida con parámetros: ClustalW (Alineamiento), Built-in Curer (Alignment curation), TNT (Filogenia), y TreeDyn (representación del árbol):

https://www.dropbox.com/s/85ig3bg52ss38xo/foto%202.jpg?dl=0
https://www.dropbox.com/s/ow56luffqli1kiq/2.pdf?dl=0

# En ausencia de la etapa de Alingment Curation:

https://www.dropbox.com/s/n4oy6k268g4uk6x/foto%203.jpg?dl=0

https://www.dropbox.com/s/yl9qe5kzwof4sda/3.pdf?dl=0

# En ausencia de la etapa de Alingment Curation:

https://www.dropbox.com/s/j16h38bzg3nbwmu/foto%204.jpg?dl=0

https://www.dropbox.com/s/ae0glmr0rnuh3da/4.pdf?dl=0

#  ¿A qué se refiere el paso de Alignment curation y para qué sirve?

El programa Gblocks realiza el paso de “Alignment Curation”, el cual consta en que el programa elimina posiciones alineadas de forma pobre y además regiones divergentes, en otras palabras, remueve el “ruido” del alineamiento. Entonces, Gblocks identifica porciones del alineamiento para eliminar posiciones con gaps, incluyendo regiones que no están presentes en todas las secuencias. Si se encuentra un alineamiento ambiguo adyacente de forma inmediata al gap, esa posición también puede ser excluida del alineamiento final, ya que el evento indel puede ser el responsable de la ambigüedad observada. 

# ¿Cuál es la diferencia entre BioNJ y Neighbor? 

Al dirigirse hacia la documentación del portal, BioNJ y Neighbor, ambos utilizan PHYLYP, el cual es un paquete de programas para inferir filogenias, pero se diferencian en la limitación en el número de taxas, que se refiere a un conjunto de organismos emparentados y agrupados de acuerdo a una clasificación, tomando en cuenta las variables entre especies cuando se realiza un alineamiento. Entonces, el programa BioNJ, puede soportar hasta <5000 taxas, mientras que Neighbor puede tolerar hasta <500 taxas; esto quiere decir la cantidad de taxas que el programa analizará antes de "confundirse", es decir, existe un límite que el programa puede soportar respecto a la cantidad de datos que se adjunten. 

# Corre de nuevo las filogenias pero esta vez sin Alignment curation. ¿Cuál es el efecto en las filogenias?

En la de ProbCons, GBlocks, MrBayes TreeDyn se puede ver una pequeña diferencia en las medida  de las ramas. La rama de arriba se reduce con la curación y la de abajo se alarga con la curación.
En la de ClustalW, remove positions with gaps, TNT y TreeDyn no hay ningún efecto en la filogenia.




