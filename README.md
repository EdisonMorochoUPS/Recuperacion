# Explicacion del proceso obtenido
Recuperacion de materia

-------------------------- 1 --------------------------

Actualizamos los paquetes instalados en su version mas reciente
<img width="732" height="348" alt="image" src="https://github.com/user-attachments/assets/eb624e63-d6c3-4b2b-b4a3-4174d573d9b9" />

-------------------------- 2 --------------------------

Comenzamos con la instalacion de Docker en nuestra distribucion de linux
<img width="959" height="364" alt="image" src="https://github.com/user-attachments/assets/a72e362a-da86-4654-abf3-f93a13f4d5bd" />

-------------------------- 3 --------------------------

Pegamos las instrucciones de instalacion en nuestra terminal para proceder a su instalacion
<img width="536" height="306" alt="image" src="https://github.com/user-attachments/assets/99a0a17e-ba35-4d17-9861-aabf3dff37fc" />

-------------------------- 4 --------------------------

Probamos docker con una imagen que ya esta predeterminadad para saber si se realizo con exito la instalacion correctamente
<img width="598" height="387" alt="image" src="https://github.com/user-attachments/assets/46629c28-a628-4889-92b6-961b333abb01" />

-------------------------- 5 --------------------------

Creamos una imagen de docker y escribimos el siguiente comando para obtener la ip de nuestra imagen que es la 172.17.0.2 por defecto
<img width="434" height="91" alt="image" src="https://github.com/user-attachments/assets/08623972-50d1-456b-a8ec-e948989739ee" />

-------------------------- 6 --------------------------

De desde nuestra terminal en kali podemos ver que si lanzamos un ping a la ip de nuestra imagen en docker vemos que se ha realizado correctamente la conexion
<img width="792" height="213" alt="image" src="https://github.com/user-attachments/assets/b11db050-b7b5-42bf-a33c-e0fba740436d" />

-------------------------- 7 --------------------------

Realizamos un update para contar con los ultimos parches despues de instalar nuestro sistema para tener mas seguridad
<img width="886" height="219" alt="image" src="https://github.com/user-attachments/assets/9145896b-12ba-48f5-9a24-8ec2b20de075" />

-------------------------- 8 --------------------------

Despues de haber creado nuestra imagen en docker instalamos apache para levantar puertos como el 80 que viene predeterminado y tambien nos sirve poer si queremos crear usuarios
<img width="886" height="302" alt="image" src="https://github.com/user-attachments/assets/27c83413-3f14-45e5-9ec2-a4b691de4eea" />

-------------------------- 9 --------------------------

Inicializamos apache y introducimos la ip en nuestro navegador y vamos a ver como esta funcionando efectivamente apache en nuestro contenedor en docker
<img width="886" height="160" alt="image" src="https://github.com/user-attachments/assets/9247ff2c-5daa-4cb9-b632-add047fbdc18" />
<img width="886" height="371" alt="image" src="https://github.com/user-attachments/assets/ce950e03-04aa-4908-af63-2d06dd77f62e" />

-------------------------- 10 --------------------------

Con el comando docker images podemos ver las imagenes que hemos creado y su id para esoger que imagen correr con solo poner los 3 primeros numeros
<img width="886" height="235" alt="image" src="https://github.com/user-attachments/assets/8464e74d-8542-49ed-9860-7f80ecee8243" />

-------------------------- 11 --------------------------

Instalamos previamente nano en nuestra imagen de docker para poder editar texto porque queremos buscar dentro de la carpeta de apache el archivo que contiene
la pagina web por defecto para asi cambiarla nosotros y desplegar una nueva y quede grabada y al encontrarla veremos como esta bajo el nombre de index.html
<img width="886" height="594" alt="image" src="https://github.com/user-attachments/assets/6d0b2970-3b12-4cfa-a870-4416a3c7d6b6" />

-------------------------- 12 --------------------------

Borramos o removemos ese archivo para que con nano lanzar uno nuevo bajo lo que nosotros queremos mediante nuestro editor de texto
<img width="728" height="358" alt="image" src="https://github.com/user-attachments/assets/c72e36ec-fad4-49b9-86da-670996f69cec" />

-------------------------- 13 --------------------------

Este es el codigo que vamos a implementar para una vez ejecutado nuestra maquina de la imagen  del contenedor poder tener esta nueva
<img width="886" height="362" alt="image" src="https://github.com/user-attachments/assets/6698b47e-eea5-4597-8705-2d787151b2f7" />

-------------------------- 14 --------------------------

Previamente guardado en nuestro editor de texto, veremos que ahora al visitar la ip que se nos dio anteriormente ahora se nos va a desplegar nuestra aplicacion
satisfactoriamente
<img width="886" height="414" alt="image" src="https://github.com/user-attachments/assets/a3546260-4362-4efa-b217-8aaf455676dd" />

-------------------------- 14 --------------------------

Ahora queremos que nuestra imagen carge satisfactoriamente y siempre se este ejecutando siempre y no se caiga y para eso abrimos el docker file
y lo editamos con nuestro editor de texto nano para darles comandos que debemos dar para que previamente se cargue los servicios que estan en nuestra imagen seguido de tail -f /dev/null para una compilacion continua y nunca se caiga
<img width="694" height="245" alt="image" src="https://github.com/user-attachments/assets/a0253eb6-57aa-4a09-92d5-a8db321c7ad7" />

-------------------------- 15 --------------------------

Como ultimo paso para ya tener todo listo y guardar y hacer entrega de nuestro contenedor usamos docker buildn para crear una imagen de Docker a partir de un archivo Dockerfile, empaquetando nuestro codigo, librerias y configuraciones en una unidad para asi pasarlo a otra persona, ya que una vez construida la imagen, esta se puede exportar para su ejecucion en cualquier maquina que tenga Docker instalado y le asignamos un nombre para que se cree la nueva imagen 
<img width="886" height="421" alt="image" src="https://github.com/user-attachments/assets/330b636a-6006-4674-9f33-70b29f081963" />










