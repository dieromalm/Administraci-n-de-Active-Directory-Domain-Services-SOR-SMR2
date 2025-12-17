## ADMINISTRACIÓN DEL ACTIVE DIRECTORY
  - Primero instalamos Hyper-V dentro de nuestro ordenador.

<img width="300" height="400" alt="image" src="https://github.com/user-attachments/assets/4ce3cb5b-a095-425b-af70-7b821211c1a8" />
<img width="133" height="26" alt="image" src="https://github.com/user-attachments/assets/851a9138-b39e-4cc1-94a4-9e8f4fa82e75" />

  - Instalamos una máquina virtual en el administrador Hyper-V de Windows Server 2022.
    
<img width="943" height="707" alt="image" src="https://github.com/user-attachments/assets/6da24225-c1ca-46d7-a4b3-20961d316cdd" />

  - Configuramos también la red NAT y el Switch dentro de nuestro ordenador.

<img width="831" height="567" alt="image" src="https://github.com/user-attachments/assets/1f6f7701-76e0-4203-92b2-09ad2fe59ff6" />
<img width="758" height="231" alt="image" src="https://github.com/user-attachments/assets/f9a8c156-7e7f-46ba-a36b-e0448cd54431" />

  - Configuramos la IPv4 y el DNS.

<img width="396" height="455" alt="image" src="https://github.com/user-attachments/assets/89b62493-9c69-4ef4-be0f-a90f230c0495" />

  - Instalamos el rol de administrador de dominio de Active Directory y creamos un nuevo bosque.

<img width="813" height="585" alt="image" src="https://github.com/user-attachments/assets/fd8557a3-8c3c-4b71-9393-ce1951a49ee4" />

  - Una vez que lo instalemos todo, el servidor se reiniciará solo y tendremos ya nuestro controlador de dominio creado.

<img width="488" height="560" alt="image" src="https://github.com/user-attachments/assets/fcb84ed5-1fd4-4591-aab2-6574866590ee" />

## CREAR UN SERVIDOR MIEMBRO DEL ACTIVE DIRECTORY
  - Realizamos la instalacion de Windows Server 2022 como hemos hecho antes.
  - Ponemos la IP nueva al servidor y que se conecte con el Servidor administrador.

<img width="395" height="449" alt="image" src="https://github.com/user-attachments/assets/37205d59-bd3d-471d-a511-c44bd30011da" />

  - Y lo conectamos al dominio de nuestro servidor administrador.

<img width="321" height="380" alt="image" src="https://github.com/user-attachments/assets/2ffccb57-9de7-4862-8024-a6424174cf0e" />

## INSTALACION DE DOMINIO AD DS Y PROMOVER EL CONTROLADOR DE DOMINIO
  - Instalamos los roles de dominio.

<img width="295" height="55" alt="image" src="https://github.com/user-attachments/assets/c2754e7a-916e-45cf-8f0c-419bc1dc74db" />

  - Configuramos el controlador de dominio dentro de la configuracion de implementacion.

<img width="748" height="553" alt="image" src="https://github.com/user-attachments/assets/c69d38f3-c691-4b9b-8f2b-5d3bfaefe4bb" />

  - Instalamos el asistente de configuracion de Active Directory como hemos hecho en el anterior (se reiniciara una vez instalado y tienes que volver a iniciar sesion).

## TRANSFERENCIA DE ROLES OPERATIVOS FLEXIBLES DE UN SOLO MAESTRO
  - Clickeamos "Herramientas" y le damos a Usuarios y equipos de Active Directory.

<img width="739" height="532" alt="image" src="https://github.com/user-attachments/assets/3d69037e-6e79-463a-ad11-985d990abf98" />

  - Le hacemos click derecho al dominio y le damos a la opcion "Maestro de operaciones" y le damos al boton "Cambiar".

<img width="391" height="449" alt="image" src="https://github.com/user-attachments/assets/3f5ee245-c786-4e52-935f-f753d810f954" />

## CREE UN SITIO DE ACTIVE DIRECTORY Y CONFIGURAR LA SUBRED PARA ESE SITIO
  - Iniciamos sesion en el administrador de "TAILWIND-DC1".
  - Abrimos "Sitios y Servicios" del apartado "Herramientas".

<img width="794" height="552" alt="image" src="https://github.com/user-attachments/assets/1d679a2f-5ec1-477e-9125-ff97314508ba" />

  - Establecemos un sitio.

<img width="426" height="394" alt="image" src="https://github.com/user-attachments/assets/22e078f7-f6c5-4545-92e5-82e2ef5f275f" />

  - Creamos una nueva subred.

<img width="427" height="542" alt="image" src="https://github.com/user-attachments/assets/8eb371f5-2ff1-4dc7-9750-1352cdda5459" />

## CREAR UNIDADES ORGANIZATIVAS
  -  Creamos en "Usuarios y equipos" una unidad organizativa (Creamos 3 que son Sydney, Melbourne y Brisbane).

 <img width="187" height="209" alt="image" src="https://github.com/user-attachments/assets/dee0b5a2-2f64-49d8-8834-1cda48de8295" />

## CREA UN USUARIO
  - Damos click derecho a "Sydney" y creamos nuevo usuario.

<img width="426" height="376" alt="image" src="https://github.com/user-attachments/assets/35805970-287a-48d6-b51d-afb2c3468dd5" />
<img width="314" height="65" alt="image" src="https://github.com/user-attachments/assets/fc5ce89e-64f7-4878-a9df-1ff22c658d55" />

  - Ponemos una fecha de expiracion a la cuenta entrado a sus propiedades.

<img width="444" height="546" alt="image" src="https://github.com/user-attachments/assets/eb51fb5c-113c-4050-bffd-12c9fe159384" />

  - Copiamos el usuario creado y a partir de ello creamos otros 2 mas y los movemos a sus respectivas carpetas.

<img width="284" height="112" alt="image" src="https://github.com/user-attachments/assets/748bbbd0-47fc-4bd5-a899-5d662f28b63e" />
<img width="178" height="191" alt="image" src="https://github.com/user-attachments/assets/a8f6a4fa-1c2c-4920-98f4-7adf2847ca17" />

## CREAR EL GRUPO DE ADMINISTRADORES DE SYDNEY
  - Hacemos click derecho en el dominio "Sydney" y creamos un nuevo grupo.

<img width="470" height="426" alt="image" src="https://github.com/user-attachments/assets/382ccdf3-07f8-4106-984e-5e786cb1b38a" />

  - Una vez creado, le damos a la pestaña de "Miembros" y añadimos el grupo creado.

<img width="452" height="501" alt="image" src="https://github.com/user-attachments/assets/192e162a-3171-4e4e-acbc-03a86069be95" />

## CONFIGURAR UN USUARIO COMO UN USUARIO PRIVILEGIADO
  - Hacemos doble click en "Sydney Contrators" y agregamos un miembro que ponga "Protected users".

<img width="437" height="537" alt="image" src="https://github.com/user-attachments/assets/7bbe6f90-5290-4256-939e-6985f5695ac4" />

## DELEGAR PERMISOS DE SEGURIDAD A UNA OU A UN GRUPO DE SEGURIDAD
  - Le damos click derecho a "Sydney" y le hacemos click a "Delegar control".

<img width="649" height="487" alt="image" src="https://github.com/user-attachments/assets/cb84d182-cd2b-4038-94f7-5b88a6a89e99" />

  - Agregamos a "Sydney Administrators".

<img width="541" height="325" alt="image" src="https://github.com/user-attachments/assets/d816a71e-1340-4670-9d00-7c41ec004678" />

  - Le damos a la opcion "Restablecer contraseñas de usuario y forzar el cambio de contraseña en el próximo inicio de sesión".

<img width="495" height="389" alt="image" src="https://github.com/user-attachments/assets/40172d1b-7707-462e-811a-ed5db1db79d0" />

## CONFIGURAR EL ATRIBUTO DE CIUDAD A UN USUARIO
  - Le damos click derecho a "Sydney Constractors" y le hacemos click a "Propiedades".

<img width="404" height="386" alt="image" src="https://github.com/user-attachments/assets/4939f5a8-13b3-459e-8b36-2482c81f5631" />

  - Le damos al apartado "Direccion" y ponemos en "Ciudad: Sydney".

<img width="515" height="561" alt="image" src="https://github.com/user-attachments/assets/ae6d07cd-4ed1-4500-ac13-302cba32bf07" />

  - Le damos click derecho a "Tailwindtrader.internal" y le damos a "Buscar".

<img width="571" height="354" alt="image" src="https://github.com/user-attachments/assets/e138ca96-0724-498e-b734-47c849c056de" />

  - Le damos a "Campo" y dentro de la casilla "Usuarios" le damos a "Ciudad".

<img width="671" height="778" alt="image" src="https://github.com/user-attachments/assets/b62dbcee-7ff0-42a0-81d4-690ad826b8a2" />

  - Lo establecemos de la siguiente manera:

<img width="581" height="364" alt="image" src="https://github.com/user-attachments/assets/6bccf53c-c6b7-4aa0-a851-b1ce32392e0d" />

  - Saldra esta ventana y le daremos a "Si" para agregar el criterio que le hemos dado.

<img width="578" height="418" alt="image" src="https://github.com/user-attachments/assets/4d21766e-e3af-4923-b909-c0d04c778774" />
<img width="260" height="54" alt="image" src="https://github.com/user-attachments/assets/356754ea-b395-47cd-bdcd-af0c76a547a7" />

## DESHABILITAR EL USUARIO CONTRATISTA DE MELBOURNE
  - Entramos al OU de Melbourne y le damos click derecho a "Melbourne Contratista" y le damos a "Deshabilitar cuenta".

<img width="357" height="115" alt="image" src="https://github.com/user-attachments/assets/5d2e408d-0516-48e5-a7a9-9b0783e612f7" />

## RESTABLECER LA CONTRASEÑA DEL USUARIO BRISBANE
  - Entramos al OU de Brisbane y le hamos click derecho a "Restablecer contraseña" y le cambiamos la contraseña.

<img width="404" height="313" alt="image" src="https://github.com/user-attachments/assets/ced3f4d0-00c6-46da-96ac-3eade3756945" />

## CONFIGURAR LA POLITICA DE CONTRASEÑAS DEL DOMINIO
  - En el administrador del servidor, en "Herramientas" le damos a "Administracion de directivas de grupos".

<img width="788" height="566" alt="image" src="https://github.com/user-attachments/assets/f5331c54-ca44-4f1f-8e67-437e4aade844" />

  - Le damos click derecho a "Default Domain Policy".

<img width="424" height="468" alt="image" src="https://github.com/user-attachments/assets/1a1901ab-baf0-4be3-a183-3b961506fdc3" />

  - Entramos en "Configuracion del equipo/directivas/directivas de cuentas/directivas de contraseñas".

<img width="792" height="556" alt="image" src="https://github.com/user-attachments/assets/88505879-913f-4c35-afab-f89ea20ef674" />

  - Establecemos en "Longitud minima de la contraseña" que debe tener almenos 14 caracteres al menos.

<img width="825" height="643" alt="image" src="https://github.com/user-attachments/assets/43eb20eb-d9b7-40e9-97d7-01c19249b767" />

## CONFIGURAR UNA POLITICA DE CONTRASEÑA DE GRANO FINO
  - Vamos a "Administrador de servicio" y "Herramientas" para entras a "Administracion de Active Directory".

<img width="938" height="211" alt="image" src="https://github.com/user-attachments/assets/1e7b5c56-687c-4530-9e93-552e26ea0058" />

  - Entramos el "Tailwindtraders (local)" y entramos a "System/Password Settings Container" y le hacemos click derecho para crear una configuracion de contraseña.

<img width="928" height="586" alt="image" src="https://github.com/user-attachments/assets/254f720a-a898-4af4-b3fc-1cdc5343e113" />

  - Le establecemos la configuracion necesaria y le damos a "Aceptar".
<img width="922" height="594" alt="image" src="https://github.com/user-attachments/assets/980a41e6-d9b2-4d34-95d4-4a94c19174c8" />

  - Pero antes ten en cuenta que debemos agregar al usuario "Domain Admins" primero (tienes que crear un usuario para que te deje).

<img width="567" height="335" alt="image" src="https://github.com/user-attachments/assets/23332588-169a-458d-8eac-d5a3831eb2dd" />

## COMO HABILITAR LA PAPELERA DE RECICLAJE EN ACTIVE DIRECTORY
  - Le damos click derecho a "tailwindtraders (local)" y le damos a "Hablitar papelera de reciclaje" para darle a "Aceptar".

<img width="858" height="299" alt="image" src="https://github.com/user-attachments/assets/04ee2595-816e-4abc-a431-8ab0ee467769" />

## RESTRINGIR LA AUTENTIFICACION NTLM
  - Vamos a "Administrador de servicio" y "Herramientas" para entras a "Administracion de directiva de grupos".

<img width="938" height="658" alt="image" src="https://github.com/user-attachments/assets/4b3de416-c89d-4e88-b8ce-a177551f3e3a" />

  - Entramos a "Default Domain Controllers Policy" y le damos click derecho para editarlo.

<img width="785" height="579" alt="image" src="https://github.com/user-attachments/assets/8fc28ccf-75cb-4ff6-92ea-c1ae229cdd37" />

  - Entramos a "Opciones de seguridad" y hacemos doble click en "Seguridad de red: Restringir NTLM: Autenticación NTLM en este dominio".

<img width="758" height="262" alt="image" src="https://github.com/user-attachments/assets/885c64f5-395a-4a44-a971-31076c5e1aa7" />

  - Le damos a "Definir esta configuracion de directiva" y "Denegar todo".

<img width="477" height="530" alt="image" src="https://github.com/user-attachments/assets/16823499-bbbd-4230-8f95-e8ec1b007354" />

## ADUDITORIA DE LA GESTION DE CUENTAS DE USUARIO EN SYDNEY
  - Entrados al OU de "Sydney" y le hacemos click derecho y le damos a "Crear un GPO en este dominio y vincularlo aquí".

<img width="565" height="466" alt="image" src="https://github.com/user-attachments/assets/b72bfbae-0879-4bc6-a62a-07261e534424" />
<img width="742" height="558" alt="image" src="https://github.com/user-attachments/assets/f341dad5-6f44-421a-9111-cd5e1220799b" />

  - Entramos al "adminsitrador de cuentas" y le damos doble click a "Auditoría de gestión de cuentas de usuario".

<img width="440" height="491" alt="image" src="https://github.com/user-attachments/assets/d71f942d-33d0-4411-b8b7-5eb9c4f2c594" />

  - Una vez dentro hacemos lo siguiente de la imagen:

<img width="434" height="538" alt="image" src="https://github.com/user-attachments/assets/fb862f1d-aef5-40ae-abd1-9a6151068fb1" />

## DENEGAR EL INICIO DE SESION COMO SERVICIO
  - Entramos de nuevo al "SydneyOUPolicy" y le hacemos click derecho para editar.

<img width="867" height="602" alt="image" src="https://github.com/user-attachments/assets/f5b6c022-1b7f-4484-bc2d-eea171c401cf" />

  - Entramos en "Asignación de derechos de usuario" y le damos doble click a "Denegar inicio de sesión como servicio". 

<img width="889" height="633" alt="image" src="https://github.com/user-attachments/assets/53d11295-181d-4a6d-bfc4-4cb3e819e08f" />

  - Una vez dentro le damos al a casilla y buscamos "Sydney Adminsitrators" y le damos a aceptar.

<img width="682" height="583" alt="image" src="https://github.com/user-attachments/assets/52b2e2a4-cb2e-40dc-8138-3361b30881a9" />
