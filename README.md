# ProyectoSR-BVP-2122
Proyecto de la asignatura Servicios en Red
![image](https://user-images.githubusercontent.com/60689503/138302830-6e77eac0-6fcf-48c3-9f4b-aa3284e69a87.png)



# Índice de contenidos: 

- [Paso Número 1](#Paso-Numero-1)
- [Paso Número 2](#Paso-Numero-2)
- [Paso Número 3](#Paso-Numero-3)
- [Paso Número 4](#Paso-Numero-4)


# Autores
Este proyecto ha sido desarrollado por Pedro Barrante Vázquez.

# Licencia
Licencia de Creative Commons.

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licencia de Creative Commons" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Esta obra está bajo una <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">licencia de Creative Commons Reconocimiento-NoComercial-CompartirIgual 4.0 Internacional</a>.

# Introducción
¡Hola!, soy Pedro Barrante Vázquez, el desarrollador de este proyecto. Con el quiero mostraros un laboratorio de un montaje de una VPC hecho en AWS, espero que disfruteis de este proyecto.
# Objetivo general
El objetivo del laboratorio sería que creemos una VPC en la nube para aprender los conceptos básicos de esta misma.


![image](https://user-images.githubusercontent.com/60689503/138308444-35d67b88-e225-4b7c-a8e8-a2f83261f1ac.png)
  
# Paso Numero 1:
Nos vamos al laboratorio de Amazon:


![image](https://user-images.githubusercontent.com/60689503/138740376-1986e2e5-69ba-40bb-bcaf-588df317646a.png)



Le damos a AWS y nos llevara a la siguiente página en la cual deberemos escoger la opcion desplegable Servicios y seleccionar VPC.



![image](https://user-images.githubusercontent.com/60689503/138740845-df1aacb0-e98c-4397-a13d-1d879cab88c8.png)


Seleccionanos la opcion de Launch VPC Wizard


![image](https://user-images.githubusercontent.com/60689503/138741102-3580a15a-3a4a-4aef-a20b-5fb4a23a9f4d.png)

Escogemos la siguiente opcion y le damos a Select

![image](https://user-images.githubusercontent.com/60689503/138741483-c2bb65e8-309a-4df4-aca7-298e0db7639a.png)

Configuramos todos los siguientes pasos y creamos la VPC:


![image](https://user-images.githubusercontent.com/60689503/138743741-ffdb948b-ce2c-462b-ae25-d480615977d5.png)

Esperamos a que se cree.

![image](https://user-images.githubusercontent.com/60689503/138744486-423d60c7-34c5-49cc-80b7-81560a2fad08.png)

# Paso Numero 2:
Le damos a la opción de subredes:


![image](https://user-images.githubusercontent.com/60689503/138744817-7a0b219c-55cd-4891-ad56-b744598aee3c.png)

Y le damos a crear subred:

![image](https://user-images.githubusercontent.com/60689503/138744895-0feb313c-e11b-4be4-907a-ddd695877d20.png)

La configuramos de la siguiente manera y le damos a Crear:

![image](https://user-images.githubusercontent.com/60689503/138745151-70f1eecd-c06f-4fbc-95d2-dd03eff55038.png)

Para la segunda subred la configuramos de la siguiente manera y creamos:

![image](https://user-images.githubusercontent.com/60689503/138745338-2f754704-b8bf-4ad4-97c2-567e78b31c79.png)


Ahora nos vamos a la opción de Route Tables que nos viene en el menu:

![image](https://user-images.githubusercontent.com/60689503/138745434-fff59aee-a5ab-480d-b7b9-de3ad235b6c9.png)


Seleccionamos la subred con Main yes y VPC Lab:

![image](https://user-images.githubusercontent.com/60689503/138745704-fcb5b594-cbf9-469e-9407-f69c14fb66a3.png)

Antes de nada le cambiamos el nombre a Private Route Table:

![image](https://user-images.githubusercontent.com/60689503/138745975-684f7921-e115-4661-9296-f3a86ab4cea5.png)


Una vez hecho esto le damos a Edit subnet associations y Seleccionamos ambas subredes: Private Subnet 1 y Private Subnet 2

![image](https://user-images.githubusercontent.com/60689503/138746217-1a02207e-d290-4321-af91-6b8a9987905b.png)

Ahora selecciono  la tabla de enrutamiento con Main y No y VPC y Lab VPC y repito los mismos pasos pero esta vez escogere las subredes: Public Subnet 1 y Public Subnet 2

![image](https://user-images.githubusercontent.com/60689503/138746646-2d79a51d-26fc-4944-9222-aca3c7757ba8.png)


# Paso Numero 3:

Seleccionamos la opción Security Grups:

![image](https://user-images.githubusercontent.com/60689503/138747577-757cab85-717f-43fd-b2ff-c1d1f3611b8a.png)

Le damos a crear Security Group:

![image](https://user-images.githubusercontent.com/60689503/138747852-42a99110-c150-4a4e-aa82-45f4ceaa5387.png)

Y lo configuramos así para permitir el trafico HTTP y le damos a crear:

![image](https://user-images.githubusercontent.com/60689503/138748148-2afc75d4-cf3a-426f-a21e-a6a85dcf6108.png)


# Paso Numero 4:

Le damos a servicios y escogemos EC2:

![image](https://user-images.githubusercontent.com/60689503/138748539-46216ddb-4a32-413d-af9e-93c044aaac43.png)


Le damos a instancias y lanzar una instancia:

![image](https://user-images.githubusercontent.com/60689503/138748663-9caa6d33-95e8-4eba-b635-d09eea80fc26.png)


En la siguiente pestaña selecciono Amazon Linux:

![image](https://user-images.githubusercontent.com/60689503/138748851-503d0211-e686-4631-af6e-66ce7f076597.png)


Ponemos todo por defecto menos la seccion de red que pondremos y coonfiguraremos esto:

![image](https://user-images.githubusercontent.com/60689503/138749169-2c65b206-3fb1-4532-9114-b8604c26df00.png)


Y la seccion avanzada que tendremos que poner lo siguiente para que el trafico HTTP pueda funcionar:  

#!/bin/bash  
#Install Apache Web Server and PHP  
yum install -y httpd mysql php  
#Download Lab files  
wget https://aws-tc-largeobjects.s3.us-west-2.amazonaws.com/CUR-TF-100-ACCLFO-2/2-lab2-vpc/s3/lab-app.zip  
unzip lab-app.zip -d /var/www/html/  
#Turn on web server  
chkconfig httpd on  
service httpd start  


Seguido le damos todo por defecto hasta llegar a la seccion de etiquetas en la cual pondremos lo siguiente:

![image](https://user-images.githubusercontent.com/60689503/138749448-3c263c34-f261-4567-b748-6b8b08da50a3.png)

Y seguimos configurando hasta que lleguemos al security group y ponemos el security group que hemos creado:

![image](https://user-images.githubusercontent.com/60689503/138749686-dba628d3-cd5b-41db-af00-6e836ceb054f.png)


Nos saltara un aviso de que no podemos tener acceso a la máquina porque el puerto 22 no esta abierto y procedemos a Lanzar la instancia, nos saldra el siguiente mensaje y escogeremos lo siguiente y le daremos a lanzar:


![image](https://user-images.githubusercontent.com/60689503/138749898-373e6fa1-879b-4e97-aec4-41cbefc10467.png)


Una vez realizado esperamos que nuestra instancia tenga los dos checks pasados, en mi caso aun no se ha completado.

![image](https://user-images.githubusercontent.com/60689503/138750029-a11621fd-ee84-4134-a58a-154d71bd3620.png)

Una vez esperemos que los dos checks de la Instancia en AWS esten en verde, ya tendriamos nuestro servidor Web en funcionamiento, hasta nos podemos conectar desde el navegador a la página web usando la DNS pública (en mi caso ec2-34-220-14-118.us-west-2.compute.amazonaws.com) como se muestra en la siguiente imagen:

![image](https://user-images.githubusercontent.com/60689503/138896450-74644a39-3ce1-4d3b-ae8b-4aebf94f9c6b.png)




# Bibliografía/webgrafía
Este Proyecto esta realizado con la información obtenida de Amazon Cloud Fundations.

# Conclusiones
En conclusión crear una VPC de amazon nos puede servir para lanzar los recursos que queramos en AWS como podría ser una instancia EC2.

# Despedida y agradecimientos

Aquí finaliza este proyecto, agradecimientos a nuestro profesor Jose Luis Rodriguez Rodriguez por el curso de AWS y enseñarnos las VPC.
