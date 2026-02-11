# SERVICIOS DE DOMINIO
Seguiremos estos pasos para instalar OpenLDAP en un servidor Linux:
- Instalamos un servidor Linux dentro de nuestra maquinas y ponemos el siguiente comando para instalarlo:

<img width="723" height="257" alt="imagen" src="https://github.com/user-attachments/assets/9ff57608-48f6-4eee-a8fc-d7f32542a681" />

- Se nos abrira un menu para poner la contraseña y lo ponemos para que termine la instalacion.
- Antes de nada, hay que usar el comando "sudo nano /etc/hosts" y poner la IP de nuestro servidor.

<img width="580" height="227" alt="imagen" src="https://github.com/user-attachments/assets/f409421a-2067-4ea0-82df-a42a4b16d0ee" />


- Tambien editamos el directorio Netplan y lo configuramos de la siguiente manera:

<img width="343" height="173" alt="imagen" src="https://github.com/user-attachments/assets/1dcbc995-cd79-40cd-9efe-c73763cb4324" />

- Miramos con el comando "dpkg –L slapd | grep (cualquier archivo)" para mirar dentro del archivo que nos ha creado la instalacion por el nombre que le pongamos, destacandolos con color por el -L.

<img width="600" height="318" alt="imagen" src="https://github.com/user-attachments/assets/76990564-2029-4408-bfdf-b69021dc57c7" />
<img width="600" height="782" alt="imagen" src="https://github.com/user-attachments/assets/419b3831-b297-4d0a-bf90-204053848d2e" />
<img width="602" height="177" alt="imagen" src="https://github.com/user-attachments/assets/c4e16ae1-e3f0-4ffa-8610-51dc07e0cfdd" />
<img width="602" height="785" alt="imagen" src="https://github.com/user-attachments/assets/d31c9f94-f219-42dc-b612-fbf5fbe902b8" />

- Activamos el archivo de configuracion del servidor LPAD y cuando salga la pantalla de ello le damos a no. Una vez hecho le tenemos que poner nombre al dominio.

<img width="954" height="280" alt="imagen" src="https://github.com/user-attachments/assets/61c7537f-23cc-4649-acbf-6040d43703b6" />

-Le ponemos un nombre de organizacion.

<img width="729" height="280" alt="imagen" src="https://github.com/user-attachments/assets/4e9c759b-738a-44c5-b0e0-f9f2d4606767" />

- Una vez puesta la contraseña, en este menu ponemos no.

<img width="638" height="203" alt="imagen" src="https://github.com/user-attachments/assets/593a63fb-d743-491d-a27f-8fff880753ec" />

- Y aqui le damos que si para que cree una nueva base de datos.

<img width="940" height="203" alt="imagen" src="https://github.com/user-attachments/assets/20b31d29-d08e-40f4-8fd9-ed202e4651f7" />

- Una vez ya esto, con el servidor podemos poner estos comandos:

<img width="1014" height="263" alt="imagen" src="https://github.com/user-attachments/assets/44e7163a-59cc-4aa5-8555-a51928b03f65" />

- Creamos un grupo de configuracion llamado "grupo.ldif" y ponemos lo siguiente:

<img width="354" height="201" alt="imagen" src="https://github.com/user-attachments/assets/d4ad4c7b-3fc7-4dfb-8ec0-f71f651a125c" />

- Y añadimos el usuario que queriamos a este

<img width="899" height="91" alt="imagen" src="https://github.com/user-attachments/assets/a34a371c-2f10-44e1-b252-5ed03a7e8f3f" />

- Creamos otro .ldif para los usuarios

<img width="506" height="225" alt="imagen" src="https://github.com/user-attachments/assets/09f44e0b-bcff-4050-a209-32325805659c" />

- Y añadimos el usuario a este tambien

<img width="917" height="63" alt="imagen" src="https://github.com/user-attachments/assets/b154abee-3d6c-4b23-a304-7a79dbf9f027" />

- En el archivo "usuarios.ldif" hay que poner tambien esto para que tenga una contraseña.

<img width="191" height="18" alt="imagen" src="https://github.com/user-attachments/assets/a5fd7a24-1686-4f4d-99e7-fb377e453f5c" />

- Con el comando "ldapsearch" podemos ver el arbol en que estan los usuarios que hemos creado

<img width="876" height="172" alt="imagen" src="https://github.com/user-attachments/assets/fd0d8562-68e9-46e8-9b43-dcdcfdfdcd65" />

## INSTALACION DE PHPLDAPADMIN
- Usamos este comando para instalarlo:

<img width="947" height="226" alt="imagen" src="https://github.com/user-attachments/assets/654befeb-5a60-46a4-a7f5-827af1499436" />

- Una vez instalado, entramos dentro de "/usr/share/phpldapadmin/config/config.php" y editamos lo siguiente:

<img width="586" height="69" alt="imagen" src="https://github.com/user-attachments/assets/6bda1793-fba2-4ed3-8c03-69b31f60de07" />
<img width="586" height="69" alt="imagen" src="https://github.com/user-attachments/assets/f0962c96-5b18-446b-b2d0-ee8abdc3101b" />
<img width="586" height="69" alt="imagen" src="https://github.com/user-attachments/assets/fff0da8a-7bbc-4d46-9adf-68ac58127fba" />
