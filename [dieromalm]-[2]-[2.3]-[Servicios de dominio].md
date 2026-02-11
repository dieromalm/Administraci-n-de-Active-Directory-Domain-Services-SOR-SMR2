# SERVICIOS DE DOMINIO
Seguiremos estos pasos para instalar OpenLDAP en un servidor Linux:
- Instalamos un servidor Linux dentro de nuestra maquinas y ponemos el siguiente comando para instalarlo:

<img width="723" height="257" alt="imagen" src="https://github.com/user-attachments/assets/9ff57608-48f6-4eee-a8fc-d7f32542a681" />

- Se nos abrira un menu para poner la contraseña y lo ponemos para que termine la instalacion.
- Antes de nada, hay que usar el comando "sudo nano /etc/hosts" y poner la IP de nuestro servidor.

<img width="478" height="257" alt="imagen" src="https://github.com/user-attachments/assets/c0eb5761-0ccb-4c08-8e8b-ebf3a38a9e4e" />

- Tambien editamos el directorio Netplan y lo configuramos de la siguiente manera:

<img width="580" height="227" alt="imagen" src="https://github.com/user-attachments/assets/1a462ee3-bc08-4696-8c39-6068cd98eb01" />

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

- Una vez ya esto, con el servidor podemos poners estos comandos

<img width="1014" height="263" alt="imagen" src="https://github.com/user-attachments/assets/44e7163a-59cc-4aa5-8555-a51928b03f65" />

- 
