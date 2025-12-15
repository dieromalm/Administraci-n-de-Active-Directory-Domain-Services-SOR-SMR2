## ADMINISTRACIÓN DEL ACTIVE DIRECTORY
  - Primero instalamos Hyper-V dentro de nuestro ordenador.

<img width="300" height="400" alt="image" src="https://github.com/user-attachments/assets/4ce3cb5b-a095-425b-af70-7b821211c1a8" />
<img width="133" height="26" alt="image" src="https://github.com/user-attachments/assets/851a9138-b39e-4cc1-94a4-9e8f4fa82e75" />

  - Instalamos una máquina virtual en el administrador Hyper-V de Windows Server 2019.
    
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

  - Instalamos el asistente de configuracion de Active Directory como hemos hecho en el anterior (se reiniciara una vez instalado y tienes que volver a iniciar sesion)

## TRANSFERENCIA DE ROLES OPERATIVOS FLEXIBLES DE UN SOLO MAESTRO
  - Clickeamos "Herramientas" y le damos a Usuarios y equipos de Active Directory

<img width="739" height="532" alt="image" src="https://github.com/user-attachments/assets/3d69037e-6e79-463a-ad11-985d990abf98" />

  - Le hacemos click derecho al dominio y le damos a la opcion "Maestro de operaciones" y le damos al boton "Cambiar"

<img width="391" height="449" alt="image" src="https://github.com/user-attachments/assets/3f5ee245-c786-4e52-935f-f753d810f954" />

## CREE UN SITIO DE ACTIVE DIRECTORY Y CONFIGURAR LA SUBRED PARA ESE SITIO
  - Iniciamos sesion en el administrador de "TAILWIND-DC1"
  - Abrimos "Sitios y Servicios" del apartado "Herramientas"

<img width="794" height="552" alt="image" src="https://github.com/user-attachments/assets/1d679a2f-5ec1-477e-9125-ff97314508ba" />

  - Establecemos un sitio.

<img width="426" height="394" alt="image" src="https://github.com/user-attachments/assets/22e078f7-f6c5-4545-92e5-82e2ef5f275f" />

  - Creamos una nueva subred.

<img width="427" height="542" alt="image" src="https://github.com/user-attachments/assets/8eb371f5-2ff1-4dc7-9750-1352cdda5459" />

## CREAR UNIDADES ORGANIZATIVAS
  -  Creamos en "Usuarios y equipos" una unidad organizativa (Creamos 3 que son Sydney, Melbourne y Brisbane)

 <img width="187" height="209" alt="image" src="https://github.com/user-attachments/assets/dee0b5a2-2f64-49d8-8834-1cda48de8295" />

## CREA UN USUARIO
  - Damos click derecho a "Sydney" y creamos nuevo usuario



