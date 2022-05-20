# sales_predictions

Como parte de mi primer proyecto en un curso de Data Science en Coding Dojo tuve que generar un modelo que pueda predecir las ventas de una tienda. Esto se trabajo con los modelos vistos hasta ese momento en clase los cuales eran Regresion Lineal, KNN, Arbol de Decision y Arboles Aleatorios.

La BBDD usada obedece al siguiente diccionario:

-Item_Identifier: ID único de producto
-Item_Weight: Peso del producto
-Item_Fat_Content: Si el producto es bajo en grasas o regular
-Item_Visibility: El porcentaje del área de exhibición total de todos los productos en una tienda asignado al producto en particular
-Item_Type: La categoría a la que pertenece el producto
-Item_MRP: Precio minorista máximo (precio de lista) del producto
-Outlet_Identifier: ID único de tienda
-Outlet_Establishment_Year: El año en el que se estableció la tienda.
-Outlet_Size: El tamaño de la tienda en términos de superficie cubierta
-Outlet_Location_Type: El tipo de área en la que se encuentra la tienda
-Outlet_Type: Si el punto de venta es una tienda de comestibles o algún tipo de supermercado
-Item_Outlet_Sales: Ventas del producto en la tienda en particular. Ésta es la variable objetivo a predecir.

Esta BBDD fue analizada y paso por un proceso de limpieza y preparacion antes de usar los modelos ya que contaba con algunos valores NaN y muchas variables categoricas.

Ya que se debian predecir ventas este no era un problema de clasificacion asi que los modelos usados fueron Regresion Lineal y KNN en su version de regresor.

Lamemtablemente con los modelos vistos no se pudo obtener un buen score (el maximo usando KNN fue de 58.96% usando 26 K). Para poder aumentar este score con los modelos usados se necesitarian mas variables para alimentar el modelo ya que segun la matriz de correlacion hecha ningun input generaba un gran movimiento en el target ademas que algunos de los valores NaN eran imposibles de obtener.

Mas alla de esto. El ejercicio sirve para poder mostrar lo aprendido gasta el momento en clase, razon por la cual dejo aqui su desarrollo.
