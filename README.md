
# Ciber2019
Repo para parcial de ciberseguridad 2019


Actualización del video del exploit

Segundo link

https://drive.google.com/file/d/1nRi3Z_JsR95GNX45Nzmd3ZZ1UyWtsQFL/view?usp=sharing


#######################################################################################################################################

1) Contenido

    Uso del ## exploit/windows/ftp/wing_ftp_admin_exec ##

    Este módulo explota el intérprete Lua incorporado en la interfaz web de administración para las versiones 3.0.0 y superiores. 
    Al suministrar una solicitud POST HTTP especialmente diseñada, un atacante puede usar os.execute () para ejecutar comandos de 
    sistema arbitrarios en el destino con privilegios de SISTEMA.

2) Referencias
    URL: http://www.wftpserver.com
    URL: https://www.wftpserver.com/help/ftpserver/index.html?administrator_console.htm

3) Plataforma: Windows

4) Arquitectura: x86 (32 bits)

5) Opciones del modulo completo.

    msf > use exploit/windows/ftp/wing_ftp_admin_exec
    msf exploit(wing_ftp_admin_exec) > show targets
            ...targets...
    msf exploit(wing_ftp_admin_exec) > set TARGET <target-id>
    msf exploit(wing_ftp_admin_exec) > show options
            ...show and set options...
    msf exploit(wing_ftp_admin_exec) > exploit

##########################################################################################################################################

ALTERNATIVA Para otra plataforma.

1) Contenido 

    Uso del ## unix/ftp/vsftpd_234_backdoor ##
    El bug encontrado es una puerta trasera creada intencionadamente por el creador con el cual se puede acceder al FTP con permisos de administrador.
    El Backdoor consiste en que accediendo al FTP y poniendo de usuario 🙂 se conseguía acceso total y ejecución de comandos en el servidor al devolver una shell del sistema.

2) Referencias: http://red-orbita.com/?p=4732

3) Plataforma: Unix

4) Opciones de modulo:
    RHOSTS -> Direccion de destino sobre la que se hará el ataque
    RPORT -> Puerto de destino (21 para este caso es el ftp)


####################################################################################################################################

El video se puede encontrar en:
https://drive.google.com/file/d/1e9tSuk6HdZDskqG2W5Td_xXfEJ0tAv8s/view?usp=sharing
