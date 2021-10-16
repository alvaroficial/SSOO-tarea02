# SSOO-tarea02
#Alvaro Martinez Diaz / alvaro.martinez@alumnos.uv.cl
#A continuacion se explicara como fue posible realizar la tarea dada.
#En primera instancia se investigaron y estudiaron los comandos curl, jq y como funcionan los redireccionamientos.
#Ademas de estudiarlos por las fuentes recomendadas, se exploró sobre estos contenidos en gran profundidad y se entendio de buena manera su funcionalidad.
#Se creo un script de bash llamado script.sh. a este se le dieron los permisos para poder ejecutarse mediante el comando:$ sudo chmod +x script.sh
#En este bash primeramente se ejecuta el comando por el cual nos podemos conectar al sitio que contiene el json a trabajar mediante su link y el comando curl
#Luego se realizan pipes y se implementa el comando jq con el cual podemos ordenar nuestro json a trabar, ademas de indicarle que nos muestre solamente las caracteristicas de id e #item_name. esto seleccionado cuidadosamente y respetando los "[] e {}". finalmente nuestra instruccion termina enviando estas caracteristicas selecionadas con el jq a un nuevo #json que tendra por nombre items.json
#luego de esta instruccion se creo una secuancia logica sencilla, la cual nos dice que si el comando anterior se ejecuto de buena manera nos mostratá un mensaje de exito y de lo #contrario nos indicara que se tuvo un error.
#Finalmente luego de ejecutarse con exito se creara el json el cual podremos aplicarle el comando jq '.' script.sh y ver ordenadas los caracteres que se pedian mostrar en el nuevo #json creado
